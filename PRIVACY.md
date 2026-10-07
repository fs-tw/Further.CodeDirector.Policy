# CodeDirector 隱私政策

更新日期：2026 年 10 月 7 日

本政策說明 CodeDirector（FCD）的 Google Drive 維運功能如何處理 Google 使用者資料。此 Google OAuth 應用目前供開發者本人使用，用於備份、CI 交付產物與維運紀錄管理。

## 存取的資料與用途

經帳號擁有者授權後，CodeDirector 可存取 Google Drive 檔案與資料夾的內容及中繼資料，包括名稱、ID、大小、父資料夾、完整性核對資訊及應用自訂屬性。

資料用於建立維運分類、上傳與下載備份及 CI 交付包、核對產物完整性，以及執行指定的清理。應用要求完整 Google Drive scope，具備檢視、建立、修改與刪除檔案的能力；這不表示每次工作都會讀取整個 Drive。具體操作由工具命令及工作設定決定。

## 儲存、傳送與資料保護

OAuth 憑證與授權 token 保存於執行環境的受保護位置，不應放入 Git、交付包、公開頁面或一般操作紀錄。檔案可在帳號擁有者指定的本機、維運執行環境與 Google Drive 間傳送。操作紀錄可能包含檔案 ID、雜湊、大小及執行結果。

Google Drive 使用者資料僅用於上述維運功能，不用於廣告、販售個人資料或訓練一般用途 AI 模型。CodeDirector 對 Google 使用者資料的使用及傳送遵守 [Google API Services User Data Policy](https://developers.google.com/terms/api-services-user-data-policy)，包括 Limited Use 要求。

## 保留、刪除與撤銷授權

備份、交付包及紀錄依各工作設定保留，不存在適用所有資料的固定保留期限。

帳號擁有者可停止工具及排程、刪除 Google Drive 檔案，並在 [Google 帳號的第三方連線設定](https://myaccount.google.com/connections) 撤銷 CodeDirector 存取權。撤銷授權不會自動刪除既有雲端檔案或已下載副本；副本與 token 應由其儲存環境分別管理。對外公開分享檔案應另外取得帳號擁有者授權。

## 聯絡

政策或資料處理問題請聯絡 [further0507@gmail.com](mailto:further0507@gmail.com)。公司網站：[豐碩資訊](https://web.furthersoftware.com.tw/)。

本倉僅公開政策文件，不包含程式碼、憑證、備份、CI 交付包或使用者資料。
