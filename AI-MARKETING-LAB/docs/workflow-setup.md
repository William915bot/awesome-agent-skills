# Javia Research Agent V1 — n8n 匯入操作

## 用途
**手動執行的低風險研究流程**：同時取得 GitHub 與 Hacker News 公開資料 → 去重整理 → 將具來源的候選資料交給 AI Agent 做題目判斷 → 產出繁體中文草稿／優先級。**不會發布貼文、寄信、寫入帳戶資料，也不會執行交易。**

## 匯入與設定
1. 打開 n8n：Workflows → Import from File，選擇 `javia-market-research-v1.json`。
2. 在 **OpenAI Chat Model** 節點，連結由你自己管理的 OpenAI API Credential；API 可能產生額外費用。不要把 API key 放在 JSON/GitHub/Notion。
3. 檢查 HTTP Request 節點是否能連外到 `api.github.com` 與 `hn.algolia.com`。公開端點有速率限制，失敗時先降低頻率。
4. 先點 **Manual Trigger → Execute workflow**，檢查前兩個 HTTP Request 的回應、候選來源 URL 與 Agent 最終輸出；必要時在模型節點更新可用模型。
5. 不要先啟用排程。手動連續測試 3 次後再額外加入 Schedule Trigger 和 Notion/Google Sheets 存檔。這一版刻意不自動發布。

## 結果應包含
- 3 個值得研究的題材（說明需求、目標受眾、證據及原始 URL）
- 1 個最值得實作的微型 Agent / Workflow 實驗
- 1 個適合 Threads 和 1 個適合 LinkedIn 的內容切角
- 來源限制與需要人類複查的疑點

## 已知限制
- 此 JSON 是**已設計、未在你的 n8n 實際匯入／執行驗證**的工作流程範本。不同 n8n 版本可能需要更新節點設定。
- GitHub 搜尋是依 API 當下搜尋結果，不能取代程式碼品質、授權與資安審查。
- Hacker News 訊號不代表台灣市場需求；發文前需補上在地化調查／真實實驗。
- AI Agent 僅能利用流程餵給它的來源標題/摘要/元資料，不能憑空聲稱已讀取整份原始碼或進行完整研究。
- 一開始先把它當 Research Assistant，而非無人監督的自動行銷員。

## 下一版 V2
添加來源白名單（官方 Docs、GitHub Releases）、版本比對、去重資料庫、人工批准與文章模板；完成後才串接 Notion／Postiz。
