# 任性週報 🦍

每週星座運勢週報，包含塔羅牌解析與瑪法達週運（水瓶座、處女座、獅子座）。

## 🌐 線上網址

- **週報頁面**: https://mizzlingling.github.io/star-weekly/horoscope.html
- **主頁面**: https://mizzlingling.github.io/lingling-daily/

## ✨ 功能

- 三星座（水瓶座、處女座、獅子座）週運切換
- 每週塔羅牌解析，含愛情／事業／財運／健康評分
- 瑪法達週運原文（來源：鏡週刊）
- 幸運色、幸運數字、吉日、水晶
- 貓咪提示
- 走路金剛動畫

## 📁 檔案結構

```
star-weekly/
├── horoscope.html      # 週報主頁面（含所有資料與樣式）
├── moods/              # 金剛心情圖片 (0.png ~ N.png)
├── kingkong.png        # 備用金剛圖
└── README.md
```

## 🔄 每週更新方式

編輯 `horoscope.html` 內的 `DATA` 物件（約第 440 行），更新三個星座的：

```javascript
const DATA = {
  aquarius: {
    tarot: { desc: `...`, aspects: { love, work, money, health } },
    mafalde: { quote: '...', tip: '...' }
  },
  virgo: { ... },
  leo:   { ... }
}
```

同時更新頁面頂部的週次標籤：

```javascript
const WEEK_LABEL = '2026年第XX週 (M/D – M/D)';
```

## 🛠️ 技術

- 純 HTML / CSS / Vanilla JavaScript
- 無框架、無依賴，直接開啟即可使用

## 📄 License

Personal Project - All Rights Reserved

---

Made with 🐱 by Lingling & Claude
