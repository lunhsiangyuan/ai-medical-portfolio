[English](README.en.md) ｜ 繁體中文

# AI × 醫學：從臨床到研究的 AI 實踐

**袁倫祥 Lun-Hsiang Yuan, MD PhD**
臺大醫院雲林分院泌尿部 副主任｜教育部部定助理教授

專長：達文西機器人手術、泌尿腫瘤學、微創手術、AI 醫療系統開發

## 目錄

- [My AI Journey](#my-ai-journey)
- [成果數據](#成果數據)
- [能力總覽](#能力總覽)
  - [🔬 研究加速](#-研究加速--ai-agent-團隊協作)
  - [🎓 教學自動化](#-教學自動化)
  - [🏥 臨床 AI 工具](#-臨床-ai-工具)
  - [📊 資料分析與營運自動化](#-資料分析與營運自動化)
  - [📜 美國醫療法規研究](#-美國醫療法規研究)
  - [🌐 已上線 Web 系統](#-已上線-web-系統)
  - [🦞 OpenClaw](#-openclaw--多-agent-ai-管理平台)
  - [🤖 AI 基礎設施（PAI）](#-ai-基礎設施pai)
- [演講記錄](#演講記錄)
- [合作提案](#合作提案)

---

## My AI Journey

```
  2020-2025        2025 Q1         2025 Q4          2026 Q1          2026 NOW
  │                │                │                │                │
  ▼                ▼                ▼                ▼                ▼

  ┌──────────┐  ┌──────────┐  ┌──────────┐  ┌────────────┐  ┌────────────────┐
  │ PhD      │  │ Chatbox  │  │ Agent    │  │ Agent Teams│  │ 完整 AI        │
  │ 博士論文  │─▶│ 對話應用  │─▶│ 實作     │─▶│ + 架構開發  │─▶│ 基礎設施       │
  │          │  │          │  │          │  │            │  │                │
  │ 醫材開發  │  │ LLM 探索  │  │ 日常實踐  │  │ 多Agent協作 │  │ 60+ Skills     │
  │ LLM 分期  │  │          │  │ 公開演講  │  │ 系統化建構  │  │ 跨領域整合     │
  └──────────┘  └──────────┘  └──────────┘  └────────────┘  └────────────────┘

  成功大學          雲嘉季會        新創醫學會       臺大泌尿部        研究/教學/臨床
  醫學工程博士      LLM 原理 +      「AI 如何融入    10 Agent 協作     /法規/商業
  攝護腺癌 LLM     攝護腺癌應用     泌尿科日常」     研究產能倍增      全面覆蓋
```

### 2020–2025 — PhD：醫學工程訓練

在國立成功大學醫學工程研究所攻讀博士，接受 medical device 開發訓練。博士論文主題：LLM 在攝護腺癌分期與分類的應用。

### 2025 — 從 Chatbox 到 Agent 實作

在雲嘉泌尿科季會發表 [LLM 在醫學上的應用](slides/LLM在醫學上的應用.pdf)，探討 Transformer 原理與攝護腺癌臨床應用。隨後將 AI 從對話工具擴展到實際工作流：門診筆記自動化、PubMed 智能搜尋、文獻整理。同年在新創醫學會發表 [LLM - How I Do It](slides/新創醫學會-LLM-How-I-Do-It.pptx)，分享 Agent 實作經驗。

### 2026 — Agent Teams 與架構開發

導入 Claude Code 後，搭配 Agent Teams 建構多 Agent 協作系統與完整開發架構。在一場 [special talk](slides/ai-agent-research-talk-final.pptx) 中展示成果：一位研究者搭配 10 個 AI Agent，產出等同完整研究團隊。同時擴展至臨床工具、教學自動化、商業營運、美國醫療法規研究等各個面向。

目前已建構 **60+ 個客製化 AI Skills**，涵蓋學術研究、臨床醫療、教學、商業營運、法規分析。

> **外部驗證：** Anthropic 於 2026 年 2 月舉辦 ["Built with Opus 4.6" Claude Code Hackathon](https://www.reddit.com/r/ClaudeAI/comments/1rabi88/built_with_opus_46_a_claude_code_hackathon/)（13,000 人報名、500 人入選），五位得獎者中有四位是非工程師——[律師、心臟科醫師、音樂人、道路工程師](https://www.digitaldigging.org/p/a-lawyer-a-road-inspector-and-a-cardiologist)。這印證了一個趨勢：**具備領域專業的人，透過 AI 工具可以建構出超越傳統開發者的解決方案。**

---

## 成果數據

```
┌────────────────────────────────────────────────────────────────────┐
│                                                                    │
│  🔬 研究                                                           │
│                                                                    │
│  • MADS 攝護腺癌分類系統（5 AI Specialist）    準確率 94.4%        │
│    342 例真實患者驗證，超越傳統方法 80%                             │
│                                                                    │
│  • Female BOO 機器學習診斷模型                  AUC 0.839          │
│    525 例、49 特徵、Two-Stage Cascaded Model                       │
│                                                                    │
│  • PI-RADS 報告 AI 擷取 — 三項全球首次                             │
│    首篇中文 PI-RADS 擷取 / 首次泌尿科測試 Claude                   │
│    首次 8 欄位結構化擷取                                           │
│                                                                    │
│  • KCNJ5 Meta-analysis                                            │
│    12,456 篇文獻 → AI 自動篩選至 13 篇                            │
│                                                                    │
│  ⚡ 效率                                                           │
│                                                                    │
│  • Agent Team：20 分鐘 → 8 分鐘（45 檔案、793 行代碼一次完成）    │
│  • Lecture Producer：40 分鐘教學影片，2 小時內從零完成              │
│  • 並行處理加速 12 倍                                              │
│                                                                    │
│  🏗️ 規模                                                          │
│                                                                    │
│  • 60+ 客製化 AI Skills（學術/臨床/創作/工程/分析）                │
│  • 15+ 外部 API 整合                                              │
│  • 3 台設備協作（MacBook Pro + Mac Mini 24/7 + Cloud）             │
│  • 1,549 條跨會話記憶，741 個自動標籤                              │
│                                                                    │
│  📜 法規研究                                                       │
│                                                                    │
│  • NYSED 醫師執照 Article 131 + Part 60 全文分析                   │
│    找到 3 條替代路徑（無 USMLE 取得紐約州執照）                     │
│  • 48 筆 Board of Regents 先例資料庫（自動月更新）                 │
│  • O-1A 簽證 8 判準覆蓋分析 + 文件自動化整理                      │
│                                                                    │
│  🌐 已上線系統                                                     │
│                                                                    │
│  • 遠距醫療平台 — Stateless 架構，HIPAA 合規設計                  │
│  • 醫師個人網站 + AI Chatbot（Gemini + Telegram 即時推播）         │
│  • Middletown 城市重建計畫網站（13 頁、三語 i18n）                 │
│  • 活動報名系統（三語表單 → Google Sheets）                        │
│  • Bloomberg 風格金融分析終端（72 模組、2,844 測試）               │
│  • Pixel Office — Agent Team 即時監控儀表板                        │
│  • 餐廳營運分析（帳務、預測、VIP 分析）                            │
│  • NYSED 先例追蹤（自動爬蟲 + GitHub 月更）                       │
│                                                                    │
└────────────────────────────────────────────────────────────────────┘
```

---

## 能力總覽

### 🔬 研究加速 — AI Agent 團隊協作

一位研究者搭配多個 AI Agent，自主完成文獻搜尋、統計分析、論文撰寫等非創造性工作。

| 研究專案 | 規模 | AI 角色 |
|----------|------|---------|
| Female BOO 機器學習診斷 | 525 例，49 特徵 | 10 Agent 協作，Cascaded AUC 0.839 |
| PHI/MRI 攝護腺癌預測 | 1,296 例 | 自動迭代 10 個 ML 模型，30 分鐘完成 |
| KCNJ5 Meta-analysis | 12,456 篇文獻 | 自動篩選、資料擷取、forest plot |
| TURP Apex-Sparing | 回顧性研究 | 統計分析 + 論文撰寫自動化 |

```
                ┌─────────────────────┐
                │   研究者（袁醫師）    │
                │   研究設計 + 監督    │
                └──────────┬──────────┘
                           │
      ┌────────────────────┼────────────────────┐
      ▼                    ▼                    ▼
┌───────────────┐  ┌───────────────┐  ┌───────────────┐
│ 文獻搜尋/篩選  │  │ 統計分析      │  │ 論文撰寫      │
│ Agent         │  │ Agent         │  │ Agent         │
└───────────────┘  └───────────────┘  └───────────────┘
┌───────────────┐  ┌───────────────┐  ┌───────────────┐
│ 品質稽核      │  │ ML 訓練       │  │ 圖表生成      │
│ Agent         │  │ Agent         │  │ Agent         │
└───────────────┘  └───────────────┘  └───────────────┘
```

→ [詳細說明](projects/01-research-agent-team.md) ｜ [投影片：AI Agent 輔助臨床研究](slides/ai-agent-research-talk-final.pptx)

---

### 🎓 教學自動化

自建 Lecture Producer 系統：輸入主題 → 結構化講稿 → 投影片 → AI 語音旁白 → 完整教學影片。

實際案例：[Metastatic Bladder Cancer 2025](slides/metastatic-bladder-cancer-2025-v3.pptx) — 25 張投影片 + 40 分鐘英文旁白，2 小時內完成。

→ [詳細說明](projects/02-lecture-producer.md)

---

### 🏥 臨床 AI 工具

每天實際使用的系統，並非概念驗證。

| 工具 | 功能 | 效益 |
|------|------|------|
| OPD Note 自動化 | 門診截圖 → AI OCR → 格式化文件 | 文件時間 -80% |
| PubMed 智能搜尋 | 自然語言 → MeSH 搜尋策略 | 搜尋時間 -70% |
| 審稿輔助系統 | 期刊論文四維度系統性評估 | 深度審查 |
| 臨床指引整合 | NCCN/EAU 指引即時查詢 | 即時最新建議 |
| 醫學英語訓練 | AI 口語糾正 + TTS 發音 | 每日自動練習 |

→ [詳細說明](projects/03-clinical-ai-tools.md) ｜ [投影片：LLM - How I Do It](slides/新創醫學會-LLM-How-I-Do-It.pptx)

---

### 📊 資料分析與營運自動化

同一套 AI 系統應用於商業場景：

- **餐廳營運** — 帳務自動化、YoY 預測、VIP 分析、天氣-銷售關聯
- **活動報名** — Google Apps Script + 三語表單（英/中/日）
- **帳單解析** — 5 家銀行 PDF → 結構化資料 → 三角交叉驗證
- **生技投資** — ClinicalTrials.gov + PubMed + 財報自動整合

→ [詳細說明](projects/04-data-analytics.md)

---

### 📜 美國醫療法規研究

AI 在法規文本分析的跨領域應用：

| 領域 | 分析內容 | 成果 |
|------|----------|------|
| NYSED 醫師執照 | NY Education Law Article 131 + Part 60 | 找到 3 條無 USMLE 替代路徑 |
| O-1A 簽證 | Immigration and Nationality Act | 8 判準覆蓋分析 + 文件自動化 |
| 先例研究 | Board of Regents 歷年決議 | 48 筆先例資料庫，自動月更新 |
| FTC 合併法規 | Title IV PPA / TVPRA | 致命障礙識別 + 可行性分析 |

---

### 🌐 已上線 Web 系統

全部由 AI 輔助開發，從設計到部署。

| 系統 | 技術亮點 | 連結 |
|------|----------|------|
| 遠距醫療平台 | Stateless 架構（零 PHI 儲存）、HIPAA 合規、三語 i18n | Private |
| 醫師個人網站 + AI Chatbot | Gemini Flash 驅動、Telegram 即時推播、7 層安全防護 | [Live](https://dr-website-react.vercel.app) |
| Middletown 城市重建計畫 | 13 頁、三語（EN/ZH/JA）、多受眾展示 | [GitHub](https://github.com/lunhsiangyuan/reviving-hudson-valley) |
| Bloomberg 風格金融終端 | 72 模組、2,844 測試、Bun + TypeScript | [GitHub](https://github.com/lunhsiangyuan/fin-terminal) |
| Pixel Office 監控儀表板 | Agent Team 即時動畫監控 | [GitHub](https://github.com/lunhsiangyuan/agent-monitor) |
| 醫學英語訓練系統 | FSI 方法論、臨床情境對話 | [GitHub](https://github.com/lunhsiangyuan/medical-english-drills) |

---

### 🦞 OpenClaw — 多 Agent AI 管理平台

自建的 AI Agent 管理平台，部署於 Mac Mini 24/7 運行。

```
┌──────────────────────────────────────────────────────────┐
│                  OpenClaw 架構                             │
├──────────────────────────────────────────────────────────┤
│                                                          │
│   Gateway (Port 18789)                                   │
│   ┌──────────┐  ┌──────────┐  ┌──────────────┐          │
│   │ Agent    │  │ Model    │  │ Channel      │          │
│   │ Runtime  │  │ Selector │  │ Dispatcher   │          │
│   │ (ACPX)   │  │          │  │              │          │
│   │ 8 並行   │  │ 4 層     │  │ Telegram     │          │
│   │ Session  │  │ Fallback │  │ LINE/Signal  │          │
│   └──────────┘  └──────────┘  └──────────────┘          │
│                                                          │
│   記憶架構：SOUL / GOAL / AGENTS / MEMORY                │
│   模型：GPT-5.4 │ Gemini │ Claude │ Ollama (local)      │
│                                                          │
└──────────────────────────────────────────────────────────┘
```

| Agent | 用途 | 模型 | 通道 |
|-------|------|------|------|
| Hermes (赫密士) | 主要對話 | GPT-5.4 | LINE, Signal |
| 住院病歷 Agent | 醫療紀錄生成 | GPT-5.2 | LINE 群組 |
| Opus Agent | 高階推理 | Claude Opus | LINE 群組 |
| 龍蝦博士 | 臨床決策 | GPT-5.2 | LINE 群組 |

→ [詳細說明](projects/06-openclaw.md)

---

### 🤖 AI 基礎設施（PAI）

```
┌────────────────────────────────────────────────────────────────┐
│                    PAI 架構                                     │
├────────────────────────────────────────────────────────────────┤
│                                                                │
│  ┌──────────────┐  ┌──────────────┐  ┌──────────────┐         │
│  │ Claude Code   │  │ 60+ Skills   │  │ Agent Teams  │         │
│  │ 核心引擎      │  │ 能力模組      │  │ 多Agent協作   │         │
│  └──────┬───────┘  └──────┬───────┘  └──────┬───────┘         │
│         └─────────────────┼─────────────────┘                  │
│                           ▼                                    │
│  ┌─────────────────────────────────────────────────────────┐   │
│  │  PubMed │ Firecrawl │ Playwright │ Google Workspace     │   │
│  │  GitHub │ Vercel    │ Telegram   │ Chrome MCP           │   │
│  └─────────────────────────────────────────────────────────┘   │
│                           ▼                                    │
│  ┌──────────────┐  ┌──────────────┐  ┌──────────────┐         │
│  │ MacBook Pro   │  │ Mac Mini     │  │ Cloud        │         │
│  │ 開發主機      │  │ 24/7 服務     │  │ Vercel/CF    │         │
│  └──────────────┘  └──────────────┘  └──────────────┘         │
│                                                                │
└────────────────────────────────────────────────────────────────┘

Skills 涵蓋：學術（文獻、統計、論文、審查）/ 臨床（門診、病歷、指引）
            創作（投影片、海報、影片、動畫）/ 工程（前端、API、部署）
            分析（EDA、ML、SHAP、存活分析）
```

→ [詳細說明](projects/05-pai-infrastructure.md)

---

## 演講記錄

| 場合 | 主題 | 投影片 |
|------|------|--------|
| 2025/03 雲嘉季會 | LLM 在醫學上的應用 | [PDF](slides/LLM在醫學上的應用.pdf) |
| 2025/11 新創醫學會 | LLM - How I Do It | [PPTX](slides/新創醫學會-LLM-How-I-Do-It.pptx) |
| 2026/02 臺大泌尿部 | AI Agent 輔助臨床研究 | [PPTX](slides/ai-agent-research-talk-final.pptx) |
| 2026 | AI Research Productivity Multiplied | [PPTX](slides/AI_Research_Productivity_Multiplied.pptx) |
| 2026 | The Hybrid Medical Workforce | [PPTX](slides/The_Hybrid_Medical_Workforce.pptx) |
| 2026/03 住院醫師教學 | Metastatic Bladder Cancer 2025（AI 全自動生成） | [PPTX](slides/metastatic-bladder-cancer-2025-v3.pptx) |

---

## 合作提案

[→ AI 賦能飛天學院 — 完整合作方案](for-feitian/cooperation-proposal.md)

---

## 聯絡

**袁倫祥 Lun-Hsiang Yuan, MD PhD**

臺大醫院雲林分院泌尿部 副主任｜教育部部定助理教授

GitHub: [@lunhsiangyuan](https://github.com/lunhsiangyuan)
