# 研究報告網站

透過 GitHub Pages 發布的靜態研究報告索引網站。

## 包含報告

### 保險研究
- 陳立楷 牙科保險最佳策略分析
- 陳立楷 牙科策略 v2 — 風險自留分析
- 投資型保單知識體系
- 台灣保險產品全景圖
- 台灣保險產品推薦清單

### AI 影視研究
- AI 影視產業應用全景

## 發布到 GitHub Pages

```bash
cd /Users/wt/PyCharmMiscProject/研究報告網站

# 1. 建立 GitHub repo 並推送
gh repo create research-reports --private --source=. --push

# 2. 啟用 GitHub Pages（使用 main branch 根目錄）
gh api repos/{owner}/research-reports -X PATCH -f has_pages=true

# 或手動操作：到 GitHub repo > Settings > Pages > Source 選 "Deploy from a branch" > 選 main / root > Save

# 3. 等待 1-2 分鐘後，網站會在以下網址上線：
# https://{username}.github.io/research-reports/
```

## 新增報告

1. 將 HTML 檔放入此資料夾
2. 編輯 `index.html` 加入連結
3. commit & push
