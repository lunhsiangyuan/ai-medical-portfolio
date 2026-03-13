# 🔬 AI Agent 研究團隊

## 概述

一套基於 Claude Code 的多 Agent 協作系統，讓單一研究者能產出等同一個完整研究團隊的成果。

## 運作方式

每個研究專案由多個專業 Agent 協作完成，各 Agent 有明確分工：

```
┌─────────────────────────────────────────────────────────┐
│  Agent 名稱          │  職責                            │
├──────────────────────┼──────────────────────────────────┤
│  Literature Agent    │  PubMed 搜尋、文獻篩選、摘要整理  │
│  Statistics Agent    │  R/Python 統計分析、模型選擇       │
│  ML-Ops Agent        │  模型訓練、超參數調整、評估        │
│  Writing Agent       │  IMRAD 結構論文撰寫               │
│  Quality Agent       │  交叉驗證、數據品質檢查            │
│  Domain Expert Agent │  臨床解讀、文獻佐證               │
│  Figure Agent        │  圖表生成、排版                   │
│  Reference Agent     │  參考文獻格式化、DOI 驗證          │
│  Submission Agent    │  投稿格式檢查、Cover letter       │
│  Review Agent        │  模擬同儕審查、預先找出弱點        │
└──────────────────────┴──────────────────────────────────┘
```

## 實際研究案例

### 案例 1：Female BOO 機器學習診斷模型
- **規模**：525 位女性患者，49 個特徵變數
- **成果**：Two-Stage Cascaded Model，AUC 0.839
- **AI 貢獻**：資料清洗、特徵工程、10+ 模型比較、交叉驗證、論文初稿
- **時間節省**：估計從 6 個月壓縮到 6 週

### 案例 2：PHI/MRI 攝護腺癌預測
- **規模**：1,296 位男性患者
- **成果**：多模態預測模型
- **AI 特色**：自動迭代 10 個 ML 模型，30 分鐘完成原本需要 5-10 小時的工作

### 案例 3：KCNJ5 Meta-analysis
- **規模**：從 12,456 篇文獻篩選至 13 篇
- **AI 貢獻**：自動化文獻搜尋策略、篩選漏斗、資料擷取、forest plot

## 相關投影片

- [AI Agent 輔助臨床研究](../slides/ai-agent-research-talk-final.pptx)
- [AI Research Productivity Multiplied](../slides/AI_Research_Productivity_Multiplied.pptx)
