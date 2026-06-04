# Python 程式思維實戰營 — 網站規劃

## 專案目標

建立一個靜態官方活動頁面，部署至 GitHub Pages，提供活動介紹並以 CTA 按鈕導向 Google 表單收集報名資訊。

---

## 目標受眾

國中生（及其家長）

---

## 技術選型

| 項目 | 選擇 | 理由 |
|------|------|------|
| 架構 | 純 HTML + CSS + 少量 JS | 無需後端，最適合 GitHub Pages 靜態部署 |
| CSS 框架 | 自訂（不依賴外部框架） | 減少相依性，頁面輕量快速 |
| 字型 | Google Fonts（Noto Sans TC） | 中文顯示最佳化 |
| 部署 | GitHub Pages（`gh-pages` 分支或 `/docs` 資料夾） | 免費、穩定、零設定 |

---

## 網站結構（單頁 index.html）

```
index.html
├── <head>    字型、SEO meta、OG 標籤
├── Hero      主標題 + 口號 + 報名按鈕（錨點）
├── Why       為什麼要學程式思維？（3 個理由）
├── Faculty   師資陣容（中央大學師資）
├── Core      5 大核心素養養成
├── Curriculum 5 天課程大綱（Day 1–5）
├── Target    適合對象（國中生 3 種情境）
└── CTA       立即報名 → Google 表單按鈕 + 聯絡資訊
```

---

## 頁面各區塊設計說明

### 1. Hero 區
- 背景：深色漸層（呼應圖片的深色科技感）
- 主標題：Python 程式思維實戰營
- 副標題：從 0 開始 × 5 天實踐 × 完成你的第一個程式作品
- 強調語：程式思維，決定未來！
- CTA 按鈕：「立即報名」（scroll to 或直接跳轉 Google 表單）

### 2. Why 區
- 3 格卡片展示學程式的原因（對應圖片三個 icon 說明）

### 3. 師資陣容
- 卡片式呈現師資背景
- 強調「中央大學師資授課」、「小班教學」、「系長親擔助教」

### 4. 5 大核心素養
- 橫排 5 個 icon 卡片
- 邏輯思維力、判斷決策力、自動化能力、資料處理能力、表達溝通能力

### 5. 5 天課程大綱
- 時間軸或卡片列表，Day 1 ~ Day 5
- 每天主題 + 上下午活動說明

### 6. 適合對象
- 3 種情境的國中生描述

### 7. CTA 報名區
- 醒目報名按鈕（`<a href="GOOGLE_FORM_URL" target="_blank">`）
- 按鈕文字：「立即報名 →」
- 說明：點擊後跳至 Google 表單填寫報名資料

---

## 視覺風格

- **主色**：深藍 `#0a1628` + 亮藍 `#1e90ff`
- **強調色**：金黃 `#ffd700`（呼應圖片星星）
- **字體色**：白色為主，區塊背景交替使用淺灰
- **字型**：Noto Sans TC（標題 bold，內文 regular）
- **風格**：科技感、青少年友善、乾淨易讀

---

## GitHub Pages 部署步驟

1. 建立 GitHub repository（建議命名：`python-camp` 或 `python-bootcamp`）
2. 將 `index.html` 推送至 `main` 分支根目錄
3. GitHub repo → Settings → Pages → Source 選 `main` / `(root)`
4. 部署完成後取得網址：`https://<username>.github.io/<repo-name>/`

---

## 待確認事項（開始製作前請提供）

- [ ] Google 表單連結（報名用）
- [ ] 活動日期與地點
- [ ] 費用資訊（或「免費」）
- [ ] 主辦單位聯絡方式（email / LINE）
- [ ] 是否需要多語言（中文即可？）

---

## 檔案結構

```
/
├── index.html        主頁面（含所有區塊）
├── style.css         樣式（可內嵌於 html 或獨立）
├── 推廣圖片.jpg       可選：放在 Hero 背景或 About 區
└── README.md         GitHub 說明（選用）
```
