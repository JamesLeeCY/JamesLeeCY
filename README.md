## Chun-Yi Lee ｜ 李俊毅

**Data scientist working on high-dimensional, noisy, multimodal data — industrial sensors, finance, language, and signal.**
**專注於高維度、高雜訊、多模態資料的資料科學家 — 工業感測、金融、語言、訊號。**

我相信模型跑出好結果之後才是工作的開始。十年處理人類行為與神經影像資料的訓練，
養成一個習慣：對每一個看起來成立的結論，再多跑一次診斷。現在我把這個習慣用在
製造、金融與語言資料上。

The work starts *after* the model looks good. Ten years of behavioral and
neuroimaging data taught me to run one more diagnostic on every result that
already looks right — that habit now points at manufacturing, financial, and language data.

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
> 主張：方法選擇應該跟隨資料結構，而不是跟隨潮流。六個「看起來成立、實際不成立」的案例，包含這個專案自己的主要宣稱。
> `imbalanced classification` `concept drift` `virtual metrology` `GNN` `XGBoost` — [完整分析 →](https://jamesleecy.github.io/semiconductor-quality-ml/)

**[precision-weighted-investment-agent](https://github.com/JamesLeeCY/precision-weighted-investment-agent)** — 多代理人精度加權投資研究系統
Multi-agent system (fundamentals, news, macro/flows, supply-chain knowledge graph, technicals) that ports precision weighting from the predictive-processing framework to Taiwan-equity judgments, tested on a survivorship-bias-free universe (271 stocks, 2019–2026, 8,475 walk-forward predictions).
> 誠實結論：方向準確率低於「永遠猜上漲」，所有策略的 Sharpe 都低於 0050；精度加權在真實資料上從未奏效——估計「誰可靠」的誤差和訊號一樣大。唯一站得住的是財報 Agent 的產業內選股（IC +0.029，t 2.16），但樣本外大幅縮水、Deflated Sharpe 不顯著。規則已凍結並事先登錄評估方式，每月排程自動做前瞻驗證。
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
