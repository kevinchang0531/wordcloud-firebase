# 2026database / wordcloud-firebase

這個專案是班級互動工具與資料庫連線示範工作區，目前包含 Firebase 即時文字雲、Supabase 文字雲示範，以及 Firebase MCP / Firestore 設定筆記。

## 主要檔案

| 檔案 | 用途 |
|---|---|
| `index.html` | Firebase 文字雲輸入頁 |
| `cloud.html` | Firebase 即時文字雲展示頁 |
| `supabase-wordcloud.html` | Supabase 文字雲示範頁 |
| `firebase.json` | Firebase Hosting / Firestore 設定 |
| `firestore.rules` | Firestore 安全規則 |
| `04.5-連接-Firebase-資料庫.md` | Firebase MCP 與 Firestore 設定筆記 |
| `07-初始化班級工具工作模式.md` | Codex 專案工作模式設定筆記 |
| `AGENTS.md` | Codex 專案規則與入口 |

## Firebase

目前 Firebase project：`fir-test-4f91d`

Firestore 規則目前只開放 `wordcloud_words` 集合讀寫，其他集合預設禁止。若新增其他工具，請先修改 `firestore.rules` 並部署規則。

## 工作模式

這個專案依照 #07 懶人包設定：

- 開始工作時說「開工」。
- 結束工作時說「收工」。
- 專案固定規則看 `AGENTS.md`。
- 進度、下一步、踩坑寫在 Obsidian：`2026database/專案工作流程.md`。

## 安全原則

- 不 commit `.env`、API key、token、密碼、Firebase Admin 憑證。
- Firebase 前端 config 可以公開，但 Admin 憑證不可以公開。
- 學生資料只使用座號與班級代號，不存真名。
