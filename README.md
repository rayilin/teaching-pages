# 教學專欄（GitHub Pages 發佈 repo）

國小教學網頁的**發佈版本**。主專案（教案／簡報／動畫產線）在私有 repo `opencode-config`。

- 首頁：<https://rayilin.github.io/teaching-pages/>（單元總覽）
- 現有單元：[視力口腔檢查站](https://rayilin.github.io/teaching-pages/units/115-1-health-vision-oral/)（康軒 115 上五上健體單元一第 2 課，P26–43）

## 結構
```
index.html                     單元總覽（手動維護卡片）
units/<英文代號>/               各單元（= 主 repo 的「教學網頁」資料夾）
.github/workflows/pages.yml    發佈流程
```

## 新增單元
1. 主 repo 完成該單元 → 把 `教學網頁/` 內容複製到 `units/<新代號>/`
2. 在根目錄 `index.html` 加一張卡片（封面用該單元 `slides/slide01.jpg`）
3. push → Pages 自動發佈

## 發佈規則
- **一律排除 `server.js`／`questions.json`／`*.bat`**（`questions.json` 含答案）；workflow 每次都會自動刪除
- 對戰後端在私有 repo `rayilin/teaching-battle`（Render），服務網址填在單元的 `battle-api.js`
- 簡報／插畫為自製或 AI 生成素材；參考影片以連結原 YouTube 頻道方式使用，版權屬原作者
