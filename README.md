# jsonwebtoken-test
-----------------------------


## JWT 組成
JWT 是一組字串，透過（.）切分成三個為 Base64 編碼的部分：
*  Header：含 Token 的種類及產生簽章（signature）要使用的雜湊演算法
*  Payload：帶有欲存放的資訊（例如用戶資訊）
*  Signature：編譯後的 Header、Payload 與密鑰透過雜湊演算法所產生

------------------------------

##Header
Header 是一個包含定義 Token 種類（type）及雜湊演算法（alg）資訊的 JSON。
在此設定Token種類為 JWT、產生簽章（signature）要使用的雜湊演算法為 HS256。
此JSON將被轉換成 Base64 編碼，成為第一個部分：

------------------------------


#Payload
Payload也是一個JSON，使用者和相關的資訊都可以放置其中。
通常會使用exp設定Token到期的時間、iat設定Token簽發時間。
最後再被轉換成Base64編碼，成為第二個部分：


------------------------------

