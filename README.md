# 🔬 實驗室營運工具箱 (Lab Operations Toolbox)

**輕量級學術策略與實驗設計畫布 (Lab Strategy & EDC Canvas Web App)**

> A lightweight Web App for Academic Strategy, Experiment Design, and Lab Management using Google Sheets & GAS.

這是一個利用 **Google Sheets** 作為隱形資料庫、透過 **Google Apps Script (GAS)** 部署的滿版網頁應用程式。
專為需要頻繁調整專案策略、設計實驗架構、管理核心設施或實驗室營運的研究人員所設計。

系統底層核心算法與網頁結構已由開發者託管於中央大腦中，使用者端僅需引入乾淨的開源「空殼 Proxy 橋樑」，即可在個人雲端硬碟中安全、獨立地跑起完全滿版的精美策略畫布，兼具**極致安全**與**一鍵無縫升級**的優勢。

---

### 四大核心管理模組：

1. **策略面 (Strategic)：** 商業模式畫布 (Business Model Canvas, BMC) 與 SWOT 分析
2. **實驗面 (Experiment)：** 實驗設計畫布 (Experiment Design Canvas, EDC)
3. **執行面 (Execution)：** OKR 研究目標管理與艾森豪重要/緊急任務矩陣 (Eisenhower Matrix)
4. **管理面 (Management)：** Risk Matrix 風險評估矩陣、Decision Log 重要決策日誌與 Retrospective 專案學習回顧

---

## 💡 核心優勢 (Key Features)

* **智財權與機密 100% 自主管理**
  免架設伺服器！採用你個人的 Google Sheets 當作隱形資料庫，所有研究計畫與機密策略 100% 存在你個人的 Google Drive 中。
* **滿版獨立網頁體驗**
  揮別擠在試算表側邊欄或小視窗的侷限，部署後擁有專屬的滿版網頁儀表板，給你的實驗設計應有的視覺尊重。
* **極速非同步自動存檔**
  像貼便利貼一樣，點擊網頁區塊直接打字。滑鼠游標移開立即觸發背景自動同步，不影響打字流暢度，更不怕資料遺失。
* **AI 擴充功能友善**
  網頁原生內容區塊 (`contenteditable`) 能完美銜接瀏覽器上的 AI 擴充功能（如 Claude、ChatGPT 等），直接喚出 AI 幫忙潤飾計畫，一起腦力激盪。
* **完全自訂標題欄位**
  支援從試算表直接更改所有九宮格與矩陣的中英文字段，無痛打造你專屬的學術戰略畫布。
* **科研友善雲端匯出**
  網頁端一鍵產生 Quarto (`.qmd`) 簡報原始碼或 PNG 圖檔，並全自動備份至你的雲端硬碟根目錄或利用 Gmail 自動寄給自己，無縫貼進計畫書草稿！

## 🚀 部署教學 (3 步驟，30 秒極速完工)

受惠於 Google Sheets 副本機制，資料庫 Library 設定會隨檔案一併完整複製，您無需手動設定任何程式碼！

### 步驟一：一鍵複製母範本 (內建完成所有配置)

1. 點擊下方連結，並點選 **「建立副本」**，將系統下載到你個人的 Google 雲端硬碟：
   👉 [一鍵建立 Google Sheet 專屬範本副本](https://docs.google.com/spreadsheets/d/1xOC0zmpLPJvnkBsGuf_mCBbY91rk310ckK9fP85g7BY/copy)

### 步驟二：一鍵自動生成系統結構

1. 打開你剛剛複製出來的那張 Google 試算表網頁，並**重新整理網頁 (F5)**。
2. 稍等 2~3 秒，上方工具列會全自動多出一個 **`🔬 科研畫布工具`** 選單。
3. 點選 **`🚀 1. 一鍵初始化系統結構`**。
4. 依據 Google 提示完成第一次執行的帳號安全授權。*(基本安全授權完成後，請「再點擊一次」該按鈕)*。
5. 試算表就會全自動幫你長出 `Strategic`、`Experiment`、`Execution`、`Management` 四個分頁與完整的底層 ID 結構。

### 步驟三：發布你個人的獨立滿版網頁 App

1. 點選試算表上方選單的 **「擴充功能」 > 「Apps Script」**。
2. 進入編輯器後，直接點擊右上方藍色的 **「部署」 > 「新增部署作業」**。
3. 點擊左上角齒輪圖示，選取 **「網頁應用程式 (Web app)」**。
4. 調整關鍵安全權限參數：
   * **執行身分 (Execute as)**：務必選取 **「存取網頁的使用者 (User accessing the web app)」** *(這能確保系統在備份檔案與寄信時，使用的是你自己的 Google 雲端配額，完全保護你的資料隱私)*。
   * **誰可以存取 (Who has access)**：選取 **「任何人 (Anyone)」**。
5. 點擊 **「部署」**。
6. 🎉 部署成功！系統會產生一段專屬你的 **網頁應用程式 URL**。點開該網址，即可開始在完全滿版的精美畫面中規劃你的科研大局！

---

## 🛠️ 進階技巧：一鍵為資料庫瘦身加速

為了讓滿版網頁的載入與即時自動存檔達到「秒開」等級，建議定期清除試算表中多餘的幽靈空白列：

1. 打開你的試算表。
2. 點選上方工具列的 **`🔬 科研畫布工具` > `🧹 2. 試算表自動瘦身`**。
3. 程式會自動觸發遠端大腦的核心優化算法，將所有分頁底部用不到的數百行空白列全數清除，讓系統運作飛快！

---

## ❤️ 支持這個專案 (How to Support This Project)

如果這個畫布工具幫助你釐清了實驗室的營運方向，或節省了你整理計畫書的時間，歡迎透過以下方式支持我的持續開發與研究：

### ☕ 1. 贊助支持 (Sponsor This Project)

開發與維護開源工具需要投入許多業餘時間。如果你覺得工具好用，歡迎給我一點鼓勵！
[![Sponsor Me](https://img.shields.io/badge/Sponsor-Support_My_Work-FFDD00?style=for-the-badge&logo=kofi&logoColor=black)](https://ko-fi.com/jingyuanchen)

### 📄 2. 學術交流 (Academic Connection)

身為生醫研究人員與病理獸醫師，若你在研究、核心設施管理中使用了本工具，或對單細胞轉錄體定序 (scRNA-seq)、空間轉錄組學 (Spatial Transcriptomics)、ONT Nanopore 定序與病原監測技術有興趣，歡迎參考或隨時與我進行學術討論與交流。

---

## ⚠️ 免責聲明 (Disclaimer)

* 本專案為開發者基於個人興趣於非工作時間所開發之開源輔助工具，與所屬之研究機構或任職單位無關。
* 專案採「現狀 (as-is)」提供，開發者與所屬機構不承擔系統維護、資料保管或任何直接/間接損害之背書與賠償責任。
* 使用者應自行妥善保管機密策略與資料。
