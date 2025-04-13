# Taiwan Weather Display UI

![HTML Badge](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS Badge](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![Tailwind Badge](https://img.shields.io/badge/TailwindCSS-3.4.17-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white)
![JavaScript Badge](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![Axios Badge](https://img.shields.io/badge/Axios-5A29E4?style=for-the-badge&logo=axios&logoColor=white)
![GSAP Badge](https://img.shields.io/badge/GSAP-88CE02?style=for-the-badge&logo=greensock&logoColor=white)


## 專案簡介

這是一個互動式的天氣查詢小專案，使用者可從台灣各縣市選擇一地，並透過中央氣象局的開放資料 API 顯示該地即時天氣資訊。

設計風格結合動態對話框、動畫字效與可愛插圖，適合作為網頁動畫、API 串接與 GSAP 練習案例。

⚠️ 注意：本專案使用的 GSAP ScrambleText 動畫與 API 請求，建議從本地端啟動才能正確執行，建議使用 Live Server 或其他本地伺服器工具開啟 `index.html`。

---

## 功能特色

- 📍 支援台灣所有縣市的區域下拉選單
- 🔮 使用 [中央氣象局 F-C0032-001](https://opendata.cwa.gov.tw/dataset/forecast/F-C0032-001) API
- GSAP ScrambleText 動畫顯示天氣資訊
-  日文對話框逐字顯示提示文字
- 支援 reset 重播動畫與資訊顯示

---

## 使用技術

- HTML5 / CSS3 / JavaScript
- Tailwind CSS（已編譯進 output.css）
- 外部字型：Google Fonts（Comic Neue、DotGothic16、Noto Sans TC 等）
- Icon：Font Awesome 6
- 動畫：GSAP（含 ScrambleText Plugin）、Animate.css、loading.io
- API 串接：Axios

---

## API 資料來源

- **中央氣象局 F-C0032-001**：3小時逐時天氣預報。

查詢網址：
```
https://opendata.cwa.gov.tw/api/v1/rest/datastore/F-C0032-001?Authorization=YOUR_API_KEY
```

---

## 使用方式

### Tailwind CLI 啟動說明

本專案使用 Tailwind CSS CLI 方式開發，請先安裝並啟動 Tailwind 編譯：

```bash
npx tailwindcss -i ./src/input.css -o ./src/output.css --watch
```

建議搭配 VS Code Live Server 插件同步觀看畫面更新。

1. 將整份專案 clone 至本地：
```bash
git clone https://github.com/your-repo-name
```

2. 使用 VSCode 搭配 Live Server 開啟 `index.html`

3. 點擊左上方「AREAS」展開選單並選擇縣市

4. 右側顯示當前天氣預報，包括：
   - 天氣現象（wx）
   - 溫度範圍（temp）
   - 舒適度指數（ci）
   - 降雨機率（pop）

5. 點擊右上角 Reset 可重新播放動畫與對話內容

---

## 效果預覽

![weather-ui-preview](https://user-images.githubusercontent.com/your-image-preview.gif)

---

## License

本專案為學習與展示用途。

若有任何建議或回饋歡迎提出 Issue 🙌

