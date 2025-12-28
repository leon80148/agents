# 品牌指南 (Brand Guidelines)

此 Skill 提供品牌設計、視覺識別系統和品牌一致性維護的專業知識。當需要建立品牌指南、確保視覺一致性、管理品牌資產或發展品牌識別時，請運用這些指南。

## 核心原則

### 品牌策略框架
1. **目的**：品牌存在的原因
2. **願景**：品牌的發展方向
3. **使命**：品牌如何達成目標
4. **價值觀**：品牌的信念
5. **個性**：品牌的行為方式
6. **承諾**：品牌提供的價值

## 視覺識別元件

### 標誌系統
- 主要標誌
- 次要標記
- 應用程式圖示（iOS/Android 規格）
- 網站圖示
- 社群媒體頭像
- 淨空區規則
- 最小尺寸
- 使用注意事項

### 色彩系統架構
```css
/* 主要調色盤 */
--brand-primary: #[hex] /* 主角色 */
--brand-secondary: #[hex] /* 輔助色 */
--brand-accent: #[hex] /* 強調色 */

/* 功能性顏色 */
--success: #10B981
--warning: #F59E0B
--error: #EF4444
--info: #3B82F6

/* 中性色 */
--gray-50 至 --gray-900

/* 語義代幣 */
--text-primary: var(--gray-900)
--text-secondary: var(--gray-600)
--background: var(--gray-50)
--surface: #FFFFFF
```

### 字體系統
```
品牌字體：[主要選擇]
系統字體堆疊：-apple-system, BlinkMacSystemFont...

字體大小階層：
- Display: 48-72px（僅用於行銷）
- H1: 32-40px
- H2: 24-32px
- H3: 20-24px
- Body: 16px
- Small: 14px
- Caption: 12px

字體粗細：
- Light: 300（可選裝飾）
- Regular: 400（內文）
- Medium: 500（UI 元素）
- Bold: 700（標題）
```

## 品牌語調原則
1. **語調屬性**：[友善、專業、創新等]
2. **寫作風格**：[簡潔、對話式、技術性等]
3. **應該**：[使用主動語態、包容、保持正面]
4. **避免**：[避免術語、不要居高臨下、跳過陳腔濫調]
5. **範例用語**：[歡迎訊息、錯誤狀態、行動呼籲]

## 元件品牌檢查清單
- [ ] 使用正確的色彩代幣
- [ ] 遵循間距系統
- [ ] 應用適當的字體排版
- [ ] 包含微動畫
- [ ] 維護圓角標準
- [ ] 使用核准的陰影/高度
- [ ] 遵循圖示風格
- [ ] 無障礙對比度

## 資產組織結構
```
/brand-assets
  /logos
    /svg
    /png
    /guidelines
  /colors
    /swatches
    /gradients
  /typography
    /fonts
    /specimens
  /icons
    /system
    /custom
  /illustrations
    /characters
    /patterns
  /photography
    /style-guide
    /examples
```

## 快速品牌審核清單
1. 標誌使用合規性
2. 顏色準確性
3. 字體排版一致性
4. 間距統一性
5. 圖示風格遵循
6. 照片處理一致性
7. 動畫標準
8. 語調匹配

## 平台特定調整
- **iOS**：在維護品牌的同時尊重 Apple 的設計語言
- **Android**：用品牌個性實施 Material Design
- **Web**：確保響應式品牌體驗
- **社群**：適應平台限制
- **印刷**：維護實體材料的品質
- **動態**：一致的動畫個性

## 品牌實施代幣
```javascript
// 開發者設計代幣
export const brand = {
  colors: {
    primary: 'var(--brand-primary)',
    secondary: 'var(--brand-secondary)',
    // ... 完整調色盤
  },
  typography: {
    fontFamily: 'var(--font-brand)',
    scale: { /* 尺寸代幣 */ }
  },
  spacing: {
    unit: 4, // 基礎單位（px）
    scale: [0, 4, 8, 12, 16, 24, 32, 48, 64]
  },
  radius: {
    small: '4px',
    medium: '8px',
    large: '16px',
    full: '9999px'
  },
  shadows: {
    small: '0 1px 3px rgba(0,0,0,0.12)',
    medium: '0 4px 6px rgba(0,0,0,0.16)',
    large: '0 10px 20px rgba(0,0,0,0.20)'
  }
}
```

## 品牌演進階段
1. **更新**：小幅更新（顏色、字體）
2. **演進**：中度變更（標誌優化、擴展調色盤）
3. **革新**：大幅改造（新識別）
4. **延伸**：新增子品牌或產品

## 無障礙標準
- 最低 WCAG AA 合規
- 色彩對比度：4.5:1（一般文字）、3:1（大文字）
- 不要僅依賴顏色
- 使用色盲模擬器測試
- 確保跨情境的可讀性

## 常見品牌違規
- 拉伸或扭曲標誌
- 使用非品牌顏色
- 混合字體風格
- 間距不一致
- 低品質圖像資產
- 語調偏離
- 無障礙性不足的色彩組合

## 開發者交接套件
1. 品牌指南 PDF
2. Figma/Sketch 庫
3. 圖示字體包
4. 色彩調色盤（多種格式）
5. CSS/SCSS 變數
6. React/Vue 元件
7. 使用範例
