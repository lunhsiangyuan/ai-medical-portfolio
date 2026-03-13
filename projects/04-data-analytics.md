# 📊 資料分析與營運自動化

## 概述

AI 不只在研究上有用。我也將同樣的技術應用在真實世界的商業營運中。

## 案例

### 1. 餐廳營運分析 (TaiwanWay)
- 自動化帳務處理（多銀行帳單 PDF → 結構化資料）
- 年度對比 (YoY) 營收預測
- VIP 客戶分析與行銷策略
- 天氣 × 銷售關聯分析
- 損益兩平分析

### 2. 活動報名系統 (NAA Spring Recital)
- Google Apps Script 後端 webhook
- 三語系表單（英/中/日）
- 自動寫入 Google Sheets
- 免費票 vs 付費票分流（Cognito Forms）

### 3. 帳單解析 Pipeline
- 支援 5 家銀行（中國信託、國泰世華、新光、玉山、BoA）
- pdftotext + Gemini VLM 混合解析
- 三角交叉驗證確保正確性
- SQLite 資料庫 + 分析報告

### 4. 生技投資分析
- ClinicalTrials.gov 臨床試驗自動追蹤
- PubMed 文獻 × 財報數據整合
- Phase 2→3 成功率預測策略
- 自動化篩選 pipeline

## 技術棧
- **語言**：TypeScript / Python
- **框架**：Bun, Pandas, Scikit-learn
- **部署**：Vercel, Cloudflare
- **自動化**：Claude Code + Custom Skills
