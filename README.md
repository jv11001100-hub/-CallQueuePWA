# 連續撥號 PWA

這是給 iPhone Safari 使用的網頁 App。

## 主要功能
- iPhone Safari 拍照 / 選照片
- OCR 辨識姓名、電話、公司
- 手動修改辨識結果
- 名單管理
- 逐筆撥號
- 已完成 / 未接 / 稍後再打
- 未接與稍後再打移到佇列最後
- 今日統計
- 本機 localStorage 保存
- 可加入 iPhone 主畫面

## 重要限制
iPhone 不允許一般網站在電話掛斷後完全自動撥下一通。
因此使用流程是：
1. 點「撥打」
2. iPhone 系統進行電話
3. 通話結束回到本 App
4. 點「已完成 / 未接 / 稍後再打」
5. 自動顯示下一位
6. 再點一次「撥打」

## 如何使用
這個 PWA 必須放到 HTTPS 網址上，iPhone Safari 才能完整使用 Service Worker / 加入主畫面。

最簡單的部署方式可以用：
- GitHub Pages
- Netlify
- Cloudflare Pages
- Vercel

部署完成後：
Safari 開啟網址 → 分享 → 加入主畫面。

## OCR 說明
目前使用 Tesseract.js CDN。
第一次辨識時需要網路載入 OCR 元件。
