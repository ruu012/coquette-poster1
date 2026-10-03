# Day 11 · Coquette 動態海報

A3 直式動態海報（粉色粒子花紋、蕾絲邊、點狀緞帶蝴蝶結），可用鏡頭做手勢互動。

## 操作

- **F11**：全螢幕　**Esc**：退出
- 點「開啟鏡頭」：
  - 右手拇指與食指的距離 → 緞帶點的大小與疏密
  - 左手食指 → 當作滑鼠，在粒子花紋上互動
  - 左手翻面 → 蕾絲重新生長
- **H**：左右手判斷互換　**M**：鏡頭畫面左右翻轉

## 展示環境

為直式螢幕（HP Z22i 在系統中轉 90°，1080×1920）設計：白底，海報滿寬，上方正中央是鏡頭框。

## 部署到 GitHub Pages

1. 把此資料夾的**全部內容**上傳到一個 GitHub repository 的根目錄（`index.html` 要在最外層）。
2. Settings → Pages → Source 選 `Deploy from a branch`，Branch 選 `main` / `(root)`，儲存。
3. 等一兩分鐘，開 `https://<帳號>.github.io/<repo 名稱>/`。

鏡頭功能需要 **HTTPS**（GitHub Pages 預設就是），第一次使用瀏覽器會詢問鏡頭權限。

## 注意

- 需要網路：p5.js（cdnjs）與手勢模型 MediaPipe（jsdelivr / Google）從網路載入。
- 版面位置固定寫在 `index.html` 最上方的 `items` 陣列裡。
- 粒子花紋素材是 `7/pink-pattern-fast.html`（圖片已內嵌，約 1.4 MB）。
