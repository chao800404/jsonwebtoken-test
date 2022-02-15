# jsonwebtoken-test
-----------------------------


### ●JWT 組成
JWT 是一組字串，透過（.）切分成三個為 Base64 編碼的部分：
*  Header：含 Token 的種類及產生簽章（signature）要使用的雜湊演算法
*  Payload：帶有欲存放的資訊（例如用戶資訊）
*  Signature：編譯後的 Header、Payload 與密鑰透過雜湊演算法所產生

