# SeriesSync - 您的專屬追劇進度管家

**SeriesSync** 是一個輕量級、無伺服器的個人追劇進度管理網頁應用程式。專為那些同時追多部劇集、動畫，需要一個簡單介面來記錄「看到第幾集」的使用者設計。

![SeriesSync Preview](https://images.unsplash.com/photo-1593784991095-a205069470b6?q=80&w=2070&auto=format&fit=crop)
*(示意圖)*

## ✨ 核心功能

*   **📱 多使用者模式**：支援家庭成員共用。每個人擁有獨立的檔案與紀錄，爸爸的韓劇與妹妹的動漫互不干擾。
*   **🔒 極致隱私**：所有資料皆儲存在瀏覽器的 `LocalStorage` 中，不需註冊帳號，資料不出這台裝置/瀏覽器。
*   **📝 智慧匯入**：支援將雜亂的文字清單（如 `萬界仙蹤419集`、`完美世界220`）直接貼上，系統會自動解析劇名與集數並批次匯入。
*   **💾 資料備份**：支援匯出 JSON 備份檔，讓您可以將進度轉移到其他裝置。
*   **🎨 簡約介面**：使用 Tailwind CSS 打造的現代化暗色系介面，專注於進度管理，無廣告干擾。
*   **⚡ 即時反應**：基於 React + Vite 建構，操作流暢無延遲。

## 🚀 技術棧

*   **前端框架**: [React](https://react.dev/) (TypeScript)
*   **建構工具**: [Vite](https://vitejs.dev/)
*   **樣式庫**: [Tailwind CSS](https://tailwindcss.com/)
*   **圖標**: [Lucide React](https://lucide.dev/)
*   **部署**: 靜態網頁 (支援 Vercel, Netlify, GitHub Pages)

## 🛠️ 如何在本地運行

如果您懂程式開發，可以在本地電腦運行此專案：

1.  **複製專案**
    ```bash
    git clone https://github.com/您的帳號/movie-record.git
    cd movie-record
    ```

2.  **安裝依賴**
    ```bash
    npm install
    ```

3.  **啟動開發伺服器**
    ```bash
    npm run dev
    ```

4.  打開瀏覽器訪問 `http://localhost:5173`

## ☁️ 如何免費部署 (推薦使用 Vercel)

您可以輕鬆將此應用程式發布到網路上，免費且永久使用：

1.  將程式碼上傳至您的 **GitHub** 儲存庫。
2.  前往 [Vercel.com](https://vercel.com) 並註冊/登入。
3.  點擊 **"Add New..."** -> **"Project"**。
4.  選擇您的 `movie-record` GitHub 儲存庫。
5.  **Framework Preset** 選擇 `Vite`。
6.  點擊 **Deploy**。
7.  等待約 1 分鐘，您就會獲得一個專屬網址 (例如 `https://my-series-sync.vercel.app`)，可以分享給家人使用！

## 📖 使用說明

### 1. 建立使用者
首次進入時，請點擊「新增成員」建立您的個人檔案。不同使用者的資料是完全隔離的。

### 2. 新增劇集
*   **手動新增**：點擊右上角的「新增」按鈕，輸入劇名、季數與集數。
*   **批次匯入**：點擊右上角的「設定/匯入」圖示，將您的追劇清單貼上。
    *   *範例格式*：
        ```text
        萬界仙蹤419集
        妖神記第七季380集
        完美世界220
        ```

### 3. 更新進度
在卡片上直接點擊 `+` 或 `-` 按鈕來更新集數。系統會自動記錄您最後觀看的時間。

## ⚠️ 注意事項

由於資料儲存在瀏覽器 (LocalStorage) 中：
*   如果您清除瀏覽器快取 (Cache/Cookies)，資料可能會遺失。**建議定期使用「匯出備份」功能下載 JSON 檔。**
*   如果在手機瀏覽器使用，請避免使用「私密瀏覽模式」，否則關閉視窗後資料會消失。

## 📄 License

本專案採用 [MIT License](LICENSE) 授權。