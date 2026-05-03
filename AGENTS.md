# 2026database - AGENTS.md

## 專案入口

專案名稱：2026database / wordcloud-firebase
專案用途：班級互動工具與 Firebase / Supabase 連線示範，主要包含即時文字雲與資料庫連線練習。
主要工作目錄：G:\我的雲端硬碟\2026database
GitHub repo：https://github.com/kevinchang0531/wordcloud-firebase
預設 branch：master

## Obsidian 對應筆記

Obsidian vault：G:\我的雲端硬碟\secondbrain
專案駕駛艙：2026database/專案工作流程.md
收工時優先更新：同上

專案駕駛艙是 Obsidian vault 裡的一篇筆記，不是工作資料夾裡的 Markdown 檔。

## 工作桌 + 三個家

- 工作桌：G:\我的雲端硬碟\2026database
- GitHub：https://github.com/kevinchang0531/wordcloud-firebase
- Obsidian：G:\我的雲端硬碟\secondbrain + 2026database/專案工作流程.md
- Firebase：fir-test-4f91d

## 同步規則

開工時：
- 使用 `startup-sync` 流程。
- 讀本檔。
- 讀 Obsidian 駕駛艙。
- 檢查 Git 狀態。
- 不自動 pull / commit / push。

收工時：
- 使用 `shutdown-sync` 流程。
- 更新 Obsidian 駕駛艙。
- 如規則、路徑、專案邊界改變才更新本檔。
- 需要時才 commit + push GitHub。

新專案初始化時：
- 使用 `project-init-sync` 流程。
- 既有專案只補缺口，不覆蓋現有 app、Firebase 設定或 Git 歷史。

## 主要檔案

入口檔：
- `index.html`：Firebase 文字雲輸入頁。
- `cloud.html`：Firebase 即時文字雲展示頁。
- `supabase-wordcloud.html`：Supabase 文字雲示範頁。

設定檔：
- `firebase.json`：Firebase Hosting / Firestore 設定。
- `firestore.rules`：Firestore 安全規則。
- `.firebaserc`：Firebase project alias。
- `.gitignore`：Git 忽略規則。

文件：
- `README.md`：repo 對外說明。
- `04.5-連接-Firebase-資料庫.md`：Firebase MCP / Firestore 設定筆記。
- `07-初始化班級工具工作模式.md`：本專案工作模式設定依據。

部署位置：
- Firebase Hosting 設定 public directory 為專案根目錄。
- GitHub remote 指向 `kevinchang0531/wordcloud-firebase`。

## 不要做

- 不要把每日進度寫進 AGENTS.md；進度寫到 Obsidian 駕駛艙。
- 不要自動納入無關 git 變更。
- 不要把 API key、token、密碼、Firebase Admin 憑證寫進 repo。
- 不要儲存學生姓名；正式資料只用座號與班級代號。
- 不要刪除或覆蓋現有 Firebase / Supabase 示範頁，除非使用者明確要求。
