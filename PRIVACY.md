# 「這裡的意思」隱私權政策

生效日期：2026 年 7 月 29 日

這份政策說明 Chrome 擴充功能「這裡的意思」會處理哪些資料、為什麼需要，以及資料會去到哪裡。

## 先說結論

「這裡的意思」不建立帳號、不放廣告，也不把你的瀏覽資料傳送到開發者的伺服器。

只有當你選擇 Gemini、閱讀資料傳送說明、按下「我了解並同意」，並主動查字時，判斷語意所需的文字才會直接傳送給 Google Gemini。

## 1. 產品的單一目的

「這裡的意思」協助臺灣英文學習者理解一個英文單字或片語在目前文章中的意思，並可把這次用法保存在本機語意庫中供日後複習。

## 2. 擴充功能會讀取什麼

為了讓雙擊查字能在一般網頁運作，擴充功能需要網站內容存取權。程式只會在你主動選取英文時，從目前頁面取得：

- 你選取的英文文字
- 文字所在的句子
- 判斷語意所需的附近段落
- 目前頁面的標題

擴充功能不會在背景自動建立或傳送完整瀏覽紀錄，也不會讀取密碼輸入框、文字輸入框或可編輯區域中的選取內容。

## 3. 傳送給 Google Gemini 的資料

Demo 模式不會把網頁文字傳送給外部 AI。當你改用 Gemini、閱讀揭露內容並按下「我了解並同意」後，每次主動查字會把以下資料直接透過 HTTPS 傳送給 Google Gemini：

- 選取文字
- 所在句子
- 必要的附近段落
- 頁面標題

請求不包含目前網址、主機名稱、完整瀏覽紀錄或你的語意庫。請求使用 `store: false`，但 Google 如何處理資料仍取決於你的 Gemini API 方案及其當時適用的條款：

- [Gemini API Additional Terms of Service](https://ai.google.dev/gemini-api/terms)
- [Google 隱私權政策](https://policies.google.com/privacy)

## 4. 只儲存在本機的資料

以下資料儲存在 Chrome 的 `chrome.storage.local`：

- Gemini API key、模型與顯示設定
- 你是否已同意目前版本的資料傳送說明，以及同意時間
- 你停用選字功能的網站主機名稱
- 你主動保存的語意庫內容，包括用法、解釋、原句、來源標題、來源網址、來源網站、遇見次數與複習狀態

這些資料不會同步到開發者的伺服器。API key 只會由你的瀏覽器直接傳送給 Google，用來驗證你發出的 Gemini API 請求。

## 5. 分享、出售與人工讀取

開發者不出售資料、不用資料投放廣告，也不允許人工閱讀你的選取文字或語意庫。除了為了提供情境解析而直接傳送給 Google Gemini 外，不會把資料分享給其他第三方。

## 6. 你的控制方式

- 你可以只使用 Demo，不同意把文字傳送給 Gemini。
- 你可以在設定頁撤回同意；撤回後會立即切回 Demo。
- 你可以在擴充功能面板停用特定網站。
- 你可以從語意庫逐筆刪除已保存的用法。
- 你可以移除擴充功能，讓 Chrome 清除它的本機儲存資料。

## 7. 安全措施

傳送到 Gemini 的資料使用 HTTPS。API key 在設定頁預設遮蔽；正式套件不包含 API key、遠端執行程式碼或廣告追蹤程式。由於 API key 仍保存在你的 Chrome 個人資料中，請勿在共用或不受信任的電腦輸入。

## 8. 政策變更

如果資料處理方式有實質改變，開發者會更新本頁與生效日期，並在擴充功能內重新顯示揭露內容；需要時會再次取得你的明確同意。

## 9. Chrome Web Store Limited Use

本產品對資料的使用遵守 [Chrome Web Store User Data Policy](https://developer.chrome.com/docs/webstore/program-policies/limited-use)，包括 Limited Use 要求。資料只用於提供或改善使用者主動使用的情境解析與學習功能。

The use of information received from Google APIs will adhere to the Chrome Web Store User Data Policy, including the Limited Use requirements.

## 10. 聯絡方式

如果你對本政策或資料處理方式有疑問，可以透過 Instagram [@raywang.tw](https://www.instagram.com/raywang.tw/) 聯絡開發者。

