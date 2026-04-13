
- Cyber Threat Intelligence (**CTI**)
- Information Sharing and Analysis Center (**ISAC**), Information Sharing and Analysis Organization (**ISAO**)

- IoC Formats
    - OpenIOC
    - CybOX (Cyber Obeservable Expression)
    - STIX (Structured Threat Information Expression)
    - TAXII (Trusted Automated Exchange of Indicator Information)
    - MAEC (Malware Attribute Enumeration and Characterization)

- IoA (Why, Stratigic indicators, proactive)

- Hackday, Hack Forums, Hack This Site, Hak5 Forums, 0x00sec

- Threat Hunting
    - 自動化 (Automation)：利用自動化手段避免每次狩獵對手時都必須從零開始
    - 情資豐富化 (Enrichment)：確保數據具備上下文資訊，以實現有效的數據分析
    - 視覺化 (Visualization)：使用數據視覺化技術識別不同數據集之間的關聯
    - 威脅狩獵者 (Threat Hunters)：具備天然好奇心、熱情與專業工具使用技巧的專業人員，能互補整體的防禦努力

- 威脅狩獵成熟度模型 (Threat Hunting Maturity Model, HMM)
    - Level 0 (初始級 - Initial)：組織不從系統收集數據 (little or no routine data collection)，主要依賴來自開源服務的威脅情資指標，且多為痛苦之金字塔 (Pyramid of Pain) 低層級的易變資訊 (如 IP、Domains)
    - Level 1 (極小級 - Minimal)：主要依賴自動化告警，但環境可視化有所提升 (收集多種日誌)，並引入威脅情資平台 (TIP) 來豐富個別的 IoCs
    - Level 2 (程序級 - Procedural)：多數組織所處的等級，使用他人建立的分析與狩獵流程 (data analysis procedures by others)，並收集大量數據 (high level of routine data collection) 以進行最小頻率分析 (Least-frequency analysis)
    - Level 3 (創新級 - Innovative)：擁有能運用多種分析技術的威脅狩獵者，可自行開發狩獵方法而非依賴第三方程序 (create new data analysis procedures)，具備機器學習與關聯數據分析能力
    - Level 4 (領先級 - Leading)：多數狩獵方法已實現營運化並轉化為自動偵測 (automate the majority of successful data analysis procedures)，狩獵團隊致力於持續改進方法論，能有效停止並偵測對手活動

💡NIST SP 800-150：Guide to Cyber Threat Information Sharing
- 威脅狩獵最佳實踐 (Threat Hunting Best Practices)：
    - 理解環境的所有維度 (Understand all aspects of the environment)：包含通訊流、用戶權限與架構，以識別異常並揭露零時差攻擊 (Zero-day) 或跨安全邊界的攻擊
    - 建立完整的網路可視化 (Establish complete network visibility)：利用網路監控與安全解決方案了解攻擊技術並有效擊退
    - 持續更新最新技術 (Keeping updated on the latest techniques)：理解新興攻擊手段並優化應對方法
    - 槓桿現有工具與自動化 (Leverage existing tools and automation)：使用機器學習演算法快速處理大量數據，節省人力成本
    - 利用 UEBA 加速異常識別 (Use UEBA to accelerate the process of identifying suspicious behavior)：監控用戶與實體行為， spotting 與系統交互時的異常活動
    - 執行內外部掃描 (Run internal and external scans)：檢查作業系統是否過期或設備是否完成補丁更新
    - 槓桿外部威脅狩獵者 (Leveraging external threat hunters)：利用其專業知識進行滲透測試、揭露未授權活動與後門 (Backdoors)，驗證網路完整性
    - 監控暗網 (Checking the dark web)：了解駭客使用的工具及可能被濫用的資訊
    - 遵循 OODA 循環 (Follow an OODA approach)：即觀察 (Observe)、導向 (Orient)、偵測 (Detect) 與行動 (Act)