
- windows credential guardt: protect PtH


---

# harden

### Identity & Access
- disable local admin `net user administrator`
- credential guard
- NTFS [File permission, Folder permission], User Account Control (UCA)
- disable SID enumeration
- Just Enough Administration (JEA), Local Administrator Password Solution (LAPS)
### System integrity
- security baseline, security compliace toolkit (SCT)
- TPM, Securitry boot, Kernel DMA Protection
- Virtualization-based Security, Memory Integrity
### Netowrk & Connectivity
- Disable unnessary service, listening port || only open necessary service, port, app, protocal
- disable LLMNR, NetBIOS, SMB
- firewall setting, dnssec
### Execution & Code Integrity
- powersheel Contrained Language Mode (CLM), attack surfaface reduction (ASR)
- Script Block Logging, Transcription
### Storage & Persistence
- regitry monitor [Log, Autorun, MRU, UserAssit]
- Do not store LAN Manager hash value
- Local Security Authority (LSA) protection, Subsystem & Permission
### TODO
- Sticky Keys: sethc.exe, utilman.exe. tampered or protected via image file exection options (IFEO)
- printer spooler: disable print spooler service
- WMI Event Subscription: Attackers often use WMI for persistence because it doesn't leave traditional "files" on the disk.
- For the browser specifically, ensure you enable "Strict" Enhanced Tracking Protection and "Always use HTTPS" in your settings

# CLM

### Step 1: Create a Self-Signed Code-Signing Certificate
Open PowerShell as **Administrator** and run this command to create a certificate and store it in your personal "Certificates" folder.

```powershell
$cert = New-SelfSignedCertificate -Type CodeSigningCert -Subject "CN=MyLocalSigningCert" -KeyUsage DigitalSignature -FriendlyName "My Signing Cert" -NotAfter (Get-Date).AddYears(2)
```

### Step 2: Trust the Certificate
Because it's "Self-Signed," Windows doesn't trust it yet. You need to move it to the **Trusted Root** and **Trusted Publishers** stores.

```powershell
# Move to Trusted Root Certification Authorities
Move-Item -Path $cert.PSPath -Destination "Cert:\LocalMachine\Root"

# Copy to Trusted Publishers (Required for AppLocker/WDAC to trust the signer)
Copy-Item -Path "Cert:\LocalMachine\Root\$($cert.Thumbprint)" -Destination "Cert:\LocalMachine\TrustedPublisher"
```

### Step 3: Write a "Restricted" Script
Let’s write a simple script that uses **.NET code**. Normally, this would be blocked in CLM.

Save this as `test_clm.ps1`:
```powershell
# This is a .NET call that fails in Constrained Language Mode
[System.Math]::Sqrt(144)
Write-Host "Success! The signed script ran in Full Language Mode." -ForegroundColor Green
```

### Step 4: Sign the Script
Now, use the certificate you created to sign the file.

```powershell
$cert = Get-ChildItem Cert:\LocalMachine\Root | Where-Object { $_.Subject -match "MyLocalSigningCert" }
Set-AuthenticodeSignature -FilePath ".\test_clm.ps1" -Certificate $cert
```
*Note: After running this, if you open `test_clm.ps1` in Notepad, you’ll see a large block of text at the bottom—that is your digital signature.*


### Cert Troubleshoot 
```powershell
Get-ChildItem Cert:\LocalMachine\Root, Cert:\LocalMachine\TrustedPublisher | Where-Object { $_.Subject -match "MyLocalSigningCert" }
```