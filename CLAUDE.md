# 給 Claude 的工作說明

- 本 repo 的 `index.html` 是「115學年度臺南特教工程執行進度」甘特圖的**正式版本**（GitHub Pages：https://hsiang0422-star.github.io/tnmr-115-project-progress/）。
- 修改這個頁面時，一律先從本 repo 拉最新內容（`git pull origin main`）再改，不要以 claude.ai 上的「工程進度甘特圖」Artifact 為基準，那份是較舊的分支版本。
- 改完後在本機用瀏覽器確認畫面，再 commit 並推送到 `main`，GitHub Pages 會自動部署。
- 施工照片放在 `photos/`，照片清單在 `index.html` 的 PHOTOS 陣列（pid 對應工程編號）。
- 資料來源為 Google 試算表「115學年度臺南特教工程執行進度總覽」，頁面直接讀取各工程分頁；讀取失敗時顯示內建快照。
