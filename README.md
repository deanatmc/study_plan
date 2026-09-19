# 第二次模考讀書計畫｜GitHub Pages 同步版

## 部署
1. 將 `index.html`、`.nojekyll`、`data/progress.json` 上傳到 GitHub repository。
2. Repository → **Settings → Pages**，選擇從 `main` branch 根目錄部署。
3. 開啟 GitHub Pages 網址。

## 第一次同步設定
1. GitHub 建立 **Fine-grained personal access token**。
2. Repository access 只選擇存放進度的 repo。
3. Repository permissions 只需要 **Contents: Read and write**。
4. 在網頁按「GitHub 同步設定」，輸入 Owner、Repo、Branch、進度檔路徑與 Token。
5. A、B 兩台裝置填同一個資料 repo，即可互相同步。

## 同步方式
- 每次更動後約 1 秒自動同步。
- 頁面開著時每 15 秒檢查 GitHub。
- 回到分頁、視窗重新取得焦點或網路恢復時會立即同步。
- 每個欄位有最後修改時間，A/B 同時修改不同欄位時會自動合併，避免整份覆蓋。

## 安全提醒
Token **不會寫進 HTML 或 GitHub**，只儲存在該裝置瀏覽器的 localStorage。若 Pages repo 是公開的，`data/progress.json` 也會公開；若不希望進度公開，可在同步設定中改用另一個 private repository 當資料 repo。
