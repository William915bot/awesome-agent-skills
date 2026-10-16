# Curated Open-source AI & Marketing Tools

收錄日期：2026-10-16｜維護人：William / Javia AI Lab

**注意：這是連結收藏／評估索引，不是 fork、程式副本、安裝紀錄或安全審核報告。** 上游專案的授權、版本、API、付費方案、外部平台條款均需於正式使用前逐項確認。特別是 AGPL、fair-code、附加條款等。

優先順序：先用既有 Javia + Codex + n8n，新增研究工具一次只選一個；社群平台 Postiz 與 Metricool 先比較，避免兩套同時維護。

| 類別 | 專案 | 評估 | 可能用途 |
|---|---|---|---|
| Marketing & Audience | [Postiz](https://github.com/gitroomhq/postiz-app) | 候選 | 社群排程、Agent CLI、內容成效；與 Metricool 二選一 |
| Marketing & Audience | [Twenty CRM](https://github.com/twentyhq/twenty) | 觀察 | 潛在客戶與商機資料 |
| Marketing & Audience | [Chatwoot](https://github.com/chatwoot/chatwoot) | 觀察 | 多管道客戶對話匯流 |
| Marketing & Audience | [Mautic](https://github.com/mautic/mautic) | 保留 | 郵件與客戶培育；需合規同意 |
| Marketing & Audience | [listmonk](https://github.com/knadh/listmonk) | 保留 | 輕量電子報系統 |
| Marketing & Audience | [Activepieces](https://github.com/activepieces/activepieces) | 觀察 | n8n 替代品；目前不重複導入 |
| Research & Data | [Crawl4AI](https://github.com/unclecode/crawl4ai) | 實驗 | 公開網站的結構化擷取，遵守網站規範 |
| Research & Data | [Firecrawl](https://github.com/firecrawl/firecrawl) | 比較 | 抓取/爬取/API，對比 Crawl4AI 成本 |
| Research & Data | [browser-use](https://github.com/browser-use/browser-use) | 觀察 | AI 瀏覽器操作，隔離環境和權限 |
| Agent Builder | [Dify](https://github.com/langgenius/dify) | 候選 | AI 工作流 / RAG / Agent App |
| Agent Builder | [OpenAI Agents SDK](https://github.com/openai/openai-agents-python) | 候選 | Python Agent 開發框架與 tool handoff |
| Agent Builder | [Microsoft Agent Framework](https://github.com/microsoft/agent-framework) | 觀察 | C#/.NET 多 Agent 導向 |
| Agent Builder | [LangGraph](https://github.com/langchain-ai/langgraph) | 觀察 | 複雜且可恢復的 Agent 工作流 |
| Agent Builder | [CrewAI](https://github.com/crewAIInc/crewAI) | 觀察 | 角色型 multi-agent 協作 |
| Engineering | [OpenHands](https://github.com/OpenHands/OpenHands) | 觀察 | 與 Codex 比較的開源 Coding Agent |

## 實驗狀態語意
- **實驗**：本月挑選，限定範圍試用
- **候選**：需求成立後才導入
- **比較**：同一職責中只保留一套
- **觀察 / 保留**：不安裝，不投入長期維護

## 評估表（每個工具）
1. 能解決的明確問題與使用場景（無問題不裝）
2. 與現有工具功能重疊、切換成本
3. 試用所需金錢、API 花費、主機與維護成本
4. 資料安全、權限、商業授權及社群平台使用條款
5. 真實使用至少 3 次後，節省的時間與結果品質

## 規範
- 禁止複製私有資訊／API Key 到公有 repo。
- 爬取公開網站仍需檢查 robots.txt、網站條款、速率限制與著作權。
- 社群貼文與私訊採人類審核後發送，避免未同意的大量寄信與帳號風險。
