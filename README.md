# 圖說研讀與跨專業整合｜113–220 頁

此專案保存[線上互動教學網站](https://drawing-review-113-213-guide.hsujerry.chatgpt.site/)截至 2026-11-04 的靜態網站內容，供版本管理與備份。

## 教材範圍

- 網站呈現第 **113–220 頁**，共 **108 頁**。
- 新教材：第 **113–163 頁**（51 頁）。
- 原教材後段：接續為第 **164–220 頁**（57 頁）。
- 功能包含六大閱讀區、逐頁圖片、章節重點、關鍵字搜尋及 PDF 連結。

## 檔案結構

```text
dist/
  index.html          網站入口
  app.js              頁面互動與搜尋
  pages-data.js       教材索引及文字資料
  styles.css          網頁樣式
  assets/             教材圖片與 PDF
qr/
  drawing_review_qr.png       純 QR Code
  drawing_review_qr.svg       向量 QR Code
  drawing_review_qr_card.png  可分享的 QR 海報
```

## 本機預覽

在專案資料夾執行：

```bash
python3 -m http.server 8000 --directory dist
```

然後開啟 `http://localhost:8000`。網站本身不需要 Node.js 編譯。

## 發布注意事項

目前正式網站仍由 ChatGPT Sites 維護；本專案是該版本的靜態備份，不會因為後續修改 Sites 而自動同步。

如要改由 GitHub Pages 提供網站，需另外啟用 GitHub Pages 並設定發布 `dist/`。站內「原教材原始 PDF」使用既有 ChatGPT Library 連結，可能受到檔案存取權限限制；請在改用其他網域前確認連結可供目標讀者使用。

教材圖面及文字的使用與再散布請遵循原始教材權利及公司授權範圍。此備份未附加開源授權條款。
