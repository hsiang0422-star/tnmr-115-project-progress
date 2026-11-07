# 給 Claude 的工作說明

- 本 repo 的 `index.html` 是「115學年度臺南特教工程執行進度」甘特圖的**正式版本**（GitHub Pages：https://hsiang0422-star.github.io/tnmr-115-project-progress/）。
- 修改這個頁面時，一律先從本 repo 拉最新內容（`git pull origin main`）再改，不要以 claude.ai 上的「工程進度甘特圖」Artifact 為基準，那份是較舊的分支版本。
- 改完後在本機用瀏覽器確認畫面，再 commit 並推送到 `main`，GitHub Pages 會自動部署。
- 施工照片放在 `photos/`，照片清單在 `index.html` 的 PHOTOS 陣列（pid 對應工程編號）。
- 資料來源：學校原始試算表 `1ocB5KTsdMfxwsoi3hO2SZsPs2aGNNsGs_efBiMlikzY`（學校網域，無法對外公開）→ 個人帳號的公開鏡像 `1-faQIzsanySNZc-RZEr31LzLWj8eMN2rVZwyrWFOk8U`（IMPORTRANGE，分頁名稱沒有「1. 」等編號前綴）。頁面以 gviz JSONP 讀鏡像（index.html 的 SHEET_ID、TABS）。
- gviz 依多數型別決定欄位型別，少數型別格子會變空值，所以摘要列（A3:J3、A4:J4）另外單列讀取。新增工程時要同時在學校試算表、鏡像（新分頁＋IMPORTRANGE）與 TABS、PROJECTS 加上。
- K 欄「備註說明」：鏡像公式範圍須為 A1:K70；有備註的任務會在名稱旁顯示「★ 備註」、長條尾端黃色 ★、提示框標題下方以黃底框顯示備註，篩選列有「★ 有備註」。
