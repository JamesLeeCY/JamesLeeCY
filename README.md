## Chun-Yi Lee ｜ 李俊毅

**Data scientist working on high-dimensional, noisy, multimodal data — industrial sensors, finance, language, and signal.**
**專注於高維度、高雜訊、多模態資料的資料科學家 — 工業感測、金融、語言、訊號。**

我建構可以上線、也可以被量測的資料與 AI 系統：引用溯源的 RAG、多代理人研究系統、
中文對話分析，以及正式上線的報名與金流系統。十年處理神經影像與行為資料的訓練，
讓我習慣在高雜訊資料上做嚴謹的評估，現在用在製造、金融與語言資料上。

I build data and AI systems that ship and can be measured: citation-grounded RAG,
multi-agent research systems, Chinese conversation analytics, and a live registration
and payment platform. Ten years of neuroimaging and behavioral data made rigorous
evaluation on noisy data a habit — now applied to manufacturing, financial, and language data.

📍 Taipei, Taiwan ｜ 正在尋找資料科學、機器學習、AI 工程職缺
📍 Open to data science, ML, and AI engineering roles in Taiwan

---

### 代表作品 ｜ Selected work

**[paper-rag-copilot](https://github.com/JamesLeeCY/paper-rag-copilot)** — 引用溯源的 RAG 系統
A strictly citation-grounded RAG assistant with a quantified evaluation harness — and a second harness that checks whether the LLM judges doing the measuring can be trusted.
> 檢索是簡單的那一半。強制引用的 prompt + 逐字引文檢查 + 經驗證的 LLM 評審（phi4，誤放率 5% [2–15]）；章節切塊 Hit@5 100% vs 固定長度 88%；逐則稽核後補上章節標題、允許跨段引文，嚴格引用精確率 84% → 97%。所有比率都附信賴區間，可完全本地運行。
> `RAG` `hybrid search` `prompt & context engineering` `LLM-as-judge` `hallucination evaluation` `Ollama`

**[fmri-video-feature-analysis](https://github.com/JamesLeeCY/fmri-video-feature-analysis)** — 影像特徵萃取與時序對齊
Per-TR visual, motion, semantic, and object-level features from naturalistic video, extracted with OpenCV, HOG, and YOLOv8.
> 在 0.752 秒的解析度下把原始影像轉成能通過統計檢驗的特徵序列。
> `computer vision` `YOLOv8` `feature engineering` `multimodal time-series`

**[line-chat-triage](https://github.com/JamesLeeCY/line-chat-triage)** — 中文對話風險分流
Health triage over LINE work groups — six business-time-aware indicators, a non-compensatory escalation tripwire, and automated PDF reports; LINE webhook and Telegram ingestion.
> 把非結構化的中文對話紀錄，變成可排序、可行動的風險訊號。合成評估以程式埋入標準答案（初步 10 組，規則系統 + phi4 組合後風險等級 9/10 正確）；股票社群模式以 entropy 時間序列預測話題轉移（AUC 0.62 → 0.71），LLM 多空標註與人工的 Cohen's κ 最高 0.42 / 0.55。
> `Chinese NLP` `semantic entropy` `LLM labeling` `synthetic benchmark` `FastAPI`

**PACLIC 40 registration** — 國際會議線上報名與金流系統（[正式站](https://registration.linguistics.ntu.edu.tw)，repo 私有）
Registration and payment system for PACLIC 40 (Dec 2026, NTU), live since 2026-10-01: Google sign-in, student-ID review, NewebPay card payments, admin CSV export.
> 與團隊協作，我負責後端功能與上線維運：查表式計價、截止邏輯、學生證到期自動刪除、Docker Compose + Nginx 部署、CI、排程備份與還原演練。
> `TypeScript` `NestJS` `Next.js` `PostgreSQL` `Docker` `GitHub Actions`

**[semiconductor-quality-ml](https://github.com/JamesLeeCY/semiconductor-quality-ml)** — 半導體品質與良率預測
Anomaly detection and yield prediction across three public manufacturing datasets — a static snapshot (SECOM), in-process time series (PHM 2016 CMP), and a production routing graph (Bosch).
> 主張：方法選擇應該跟隨資料結構，而不是跟隨潮流。PHM CMP 官方測試集 MSE 6.24；以診斷把關模型選擇，例如 CMP 虛擬量測 R² 0.993 在主要群集內為 0.897、驗證集最佳的 1D-CNN 在測試集最差——避免把假改善帶進部署。
> `imbalanced classification` `concept drift` `virtual metrology` `GNN` `XGBoost` — [完整分析 →](https://jamesleecy.github.io/semiconductor-quality-ml/)

**[precision-weighted-investment-agent](https://github.com/JamesLeeCY/precision-weighted-investment-agent)** — 多代理人精度加權投資研究系統
Multi-agent system (fundamentals, news, macro/flows, supply-chain knowledge graph, technicals) that ports precision weighting from the predictive-processing framework to Taiwan-equity judgments, tested on a survivorship-bias-free universe (271 stocks, 2019–2026, 8,475 walk-forward predictions).
> 關鍵發現：精度加權的前提是能可靠估計各來源的準確度，實測估計誤差與訊號同量級，因此系統改以財報 Agent 為主。財報 Agent 的產業內選股有效（IC +0.029，t 2.16，各子期間與取樣起點皆為正）；選股策略的 Sharpe 尚未超越 0050，樣本外效果較小。規則已凍結並事先登錄評估方式，每月排程自動做前瞻驗證。
> `multi-agent` `LLM` `walk-forward backtesting` `information coefficient` `survivorship bias` `deflated Sharpe` `forward validation`

All projects were built with Claude Code as a development assistant. ｜ 所有專案皆以 Claude Code 協助開發。

---

### 技術 ｜ Tools

`Python` `R` `MATLAB` `SQL` `TypeScript` `JavaScript`
`scikit-learn` `XGBoost` `graph neural networks` `time-series analysis`
`RAG` `LLM evaluation` `multi-agent systems` `Ollama` `ChromaDB`
`OpenCV` `YOLOv8` `signal processing`
`FastAPI` `NestJS` `Next.js` `PostgreSQL` `Docker`
`walk-forward backtesting` `model calibration` `experimental design` `Claude Code`

---

### 背景 ｜ Background

- **業界** — 數位健康公司 R&D 專案經理：整合性失智症延緩方案，橫跨認知訓練、睡眠偵測、營養產品三個外部合作團隊，含雲端平台與 API 規劃。
  *R&D project manager at a digital health company — a three-partner dementia-delay program with cloud platform and API design.*
- **研究** — 台大 & 中研院跨領域神經科學博士候選人，預計 2027 年 3 月畢業。兩篇第一作者論文（*Journal of Psychiatry and Neuroscience* 2023、*Biological Psychology* 2021）。
  *PhD candidate, NTU & Academia Sinica, expected Mar 2027. Two first-author publications.*
- **國際** — 2024–2025 於 Brandeis University 擔任訪問學者（教育部公費），建置台美跨站點神經影像資料平台。
  *Visiting scholar at Brandeis University on a government-funded program; built a Taiwan–US cross-site data platform.*

---

### 聯絡 ｜ Contact

[chunyilee0102@gmail.com](mailto:chunyilee0102@gmail.com) ·
[LinkedIn](https://www.linkedin.com/in/chun-yi-lee-1778ab1a1/) ·
[jamesleecy.github.io](https://jamesleecy.github.io)
