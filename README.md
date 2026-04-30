# 艾爾芙卡 - 遊戲介紹網站

## 專案簡介

目前網站已整理為可直接部署到儲存庫根目錄的靜態站，適合 GitHub Pages 與 GitHub 組織站網址直接對外提供。首頁與所有主要頁面都位於最外層，資源則集中在 assets 目錄。

## 檔案結構

```
game_web/
├── index.html                   # 首頁
├── world.html                   # 世界展示
├── characters.html              # 角色展示
├── gameplay.html                # 玩法介紹
├── download.html                # 下載試玩
├── 404.html                     # 錯誤頁
├── favicon.ico
├── _headers                     # 靜態站標頭設定
├── _redirects                   # 靜態站導向設定
├── assets/
│   ├── css/
│   ├── images/
│   ├── js/
│   └── media/
├── builds/                      # 試玩包輸出目錄
├── resource/                    # 原始企劃與素材來源
├── tools/
├── README.md
├── .gitignore
└── .nojekyll                    # GitHub Pages 停用 Jekyll 處理
```

## 主要功能

### 🎮 遊戲展示區域
- **Hero區域**: 具有漸變背景和粒子效果的主視覺區域
- **遊戲Logo**: 使用您提供的LOGO.png
- **主角展示**: 展示琉波像素小人角色
- **互動按鈕**: 平滑滾動導航

### 📖 內容區塊
1. **遊戲介紹**: 故事背景和遊戲目標
2. **遊戲特色**: 6個主要特色，包含動畫效果
3. **角色介紹**: 主角和舞獅守護者的詳細介紹
4. **武器系統**: 展示遊戲中的武器特色
5. **社群媒體**: Instagram連結區域
6. **開發團隊**: ELVKA團隊介紹

### 🎨 視覺特效
- **像素藝術風格**: 所有遊戲圖片使用像素渲染
- **動畫效果**: 滾動動畫、懸停效果、打字效果
- **響應式設計**: 適配桌面和移動設備
- **粒子效果**: Hero區域的動態粒子背景
- **毛玻璃效果**: 特色卡片使用backdrop-filter

## 技術特點

### CSS 特色
- **漸變背景**: 使用CSS漸變創建視覺層次
- **Backdrop Filter**: 現代毛玻璃效果
- **CSS動畫**: 關鍵幀動畫和過渡效果
- **Flexbox/Grid**: 現代佈局技術

### JavaScript 功能
- **平滑滾動**: 錨點導航
- **滾動動畫**: 元素進入視窗時觸發動畫
- **打字效果**: 主標題的打字機效果
- **粒子系統**: 動態背景粒子
- **視差效果**: Hero區域的視差滾動

## 使用方法

1. **直接訪問**: 在瀏覽器中打開 `index.html`
2. **本地服務器**: 使用任何Web服務器（如Live Server）提供服務
3. **GitHub Pages / 組織站**: 直接以儲存庫根目錄發布，網址會從根目錄的 `index.html` 進站

## 自定義指南

### 修改文字內容
在 `index.html` 或其他同層頁面中找到相應的文字區塊進行修改：

```html
<h1 class="display-4 mb-4">琉波傳說</h1>
<p class="lead mb-4">您的遊戲描述...</p>
```

### 替換圖片
將新圖片放入 `assets/images/` 目錄，並在HTML中更新圖片路徑：

```html
<img src="assets/images/your-image.png" alt="描述">
```

### 調整樣式
在 `assets/css/game-custom.css` 中修改CSS樣式：

```css
.game-hero {
    background: linear-gradient(135deg, #your-color1, #your-color2);
}
```

### 添加新區塊
參考現有區塊的結構，添加新的內容區域：

```html
<section class="section" id="new-section">
    <div class="container">
        <!-- 您的內容 -->
    </div>
</section>
```

## 瀏覽器支援

- ✅ Chrome 88+
- ✅ Firefox 85+
- ✅ Safari 14+
- ✅ Edge 88+

## 性能優化建議

1. **圖片優化**: 壓縮PNG圖片以減少檔案大小
2. **CSS合併**: 可以將custom.css合併到主樣式檔案中
3. **JavaScript壓縮**: 生產環境使用壓縮版本
4. **CDN**: 考慮使用CDN提供靜態資源

## 後續開發建議

1. **內容管理**: 可以考慮使用CMS系統管理內容
2. **多語言支援**: 添加國際化支援
3. **SEO優化**: 添加meta標籤和結構化數據
4. **PWA功能**: 添加離線支援和安裝提示

## 聯絡資訊

如需進一步的自定義或有任何問題，請隨時聯絡我！

---

**製作日期**: 2024年10月25日  
**版本**: 1.0  
**基於**: Deadfire HTML模板