# 教學網頁（GitHub Pages 發佈 repo）

本 repo 只放**自製教學網頁的發佈版本**，主專案（含簡報／教案產線）在私有 repo `opencode-config`。

- 現有單元：[視力口腔檢查站｜康軒版五上健體](https://rayilin.github.io/teaching-pages/)（康軒 115 上五上健體單元一第 2 課，P26–43）

## 發佈規則
- 每次改動單元網頁（私有主 repo）→ 複製到本 repo 對應資料夾 → push → Pages 自動發佈
- **發佈包一律排除 `server.js`／`questions.json`／`start-battle.bat`**（`questions.json` 含答案，只放私 repo）；workflow 再做一次防呆刪除
- 簡報／插畫為 AI 自製素材；參考影片以連結到原 YouTube 頻道的方式使用，版權屬原作者
- 兩人對戰功能需區網伺服器（私 repo 內 `教學網頁/server.js`，雙擊 `start-battle.bat` 啟動），線上版顯示教室用法
