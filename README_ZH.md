# 🚀 全端即時通訊與學習平台

這是一個由我獨立開發的全端專案，整合了即時聊天、語言學習（單字/文章）與 AI 問答功能。專案採用微服務架構，展示了從前端、後端到 DevOps 的完整技能。

## 📁 專案架構與倉庫連結

本專案由三個核心服務構成，點擊連結查看各服務的詳細程式碼與說明：

| 服務名稱 | 技術堆疊 | 倉庫連結 | 核心功能 |
| :--- | :--- | :--- | :--- |
| **主後端服務** | .NET 8, MSSQL, RabbitMQ, Docker | [dotnet_chatroom_service](https://github.com/lauchiwai/dotnet_chatroom_service) | 用戶認證、單字管理、文章管理、聊天室、Outbox 模式 |
| **AI 聊天服務** | FastAPI, MongoDB, Qdrant, Docker | [py_chat_service](https://github.com/lauchiwai/py_chat_service) | 聊天記錄儲存、RAG AI 問答、向量搜尋 |
| **前端應用** | Vue 3, TypeScript, Pinia, Docker | [vue_chatroom_service](https://github.com/lauchiwai/vue_chatroom_service) | 響應式網頁、即時通訊、學習功能、雙 Token 驗證、CSP |

| 項目 | 連結 | 帳號資訊 |
| :--- | :--- | :--- |
| **前端應用 (Vue.js)** | [https://oniind244.online/](https://oniind244.online/) |  |
| **示範影片** | [https://www.youtube.com/shorts/KFJzDUnJtvw](https://www.youtube.com/shorts/KFJzDUnJtvw) |  |
| **測試帳號 1** | | **帳號：** `user01` <br> **密碼：** `a1234*` |
| **測試帳號 2** | | **帳號：** `` <br> **密碼：** `` |

## 🛠️ 技術亮點 (Technical Highlights)

### 🔐 安全與架構
- **雙 JWT 驗證系統**: 實作 Access Token 與 Refresh Token 機制，保障用戶安全與無感刷新。
- **微服務通信**: 主後端服務透過訊息佇列 (RabbitMQ) 與 AI 服務非同步溝通，實現服務解耦。
- **Outbox 模式**: 確保在分散式系統中，資料庫更新與訊息發送的最終一致性。

### ⚡ 即時性與體驗
- **Server-Sent Events (SSE)**: 用於實現即時數據推送，提供流暢的用戶體驗。
- **RAG AI 問答**: 結合 Qdrant 向量資料庫與 FastAPI，打造基於自有知識庫的智能問答機器人。
- **響應式網頁設計 (RWD)**: 前端使用 Vue 3 與 SCSS，確保在手機、平板、電腦上皆有完美體驗。

### 🚀 部署與維運 (DevOps)
- **容器化**: 所有服務均使用 Docker 容器化，便於開發、測試與部署。
- **CI/CD 流水線**: 為每個服務建立了自動化建置、測試與部署流程。
- **內容安全政策 (CSP)**: 於前端實施 CSP 標頭，有效防禦 XSS 等網路攻擊。

