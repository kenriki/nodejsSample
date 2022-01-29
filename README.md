
# Node.js の mockyを使用しスタブREST API を作成
![VSCODE画面](/img/gamen1.png) 

## 事前準備① 
> mocky のインストール  
```vim
npm install -D mocky
```
## 事前準備②  
> リクエストに応じて処理を変えるために、JSファイルを作成  
> ここでは `sample_api.js` を作成  

## 事前準備③
> JSONファイル

## 実行方法
```vim
node sample_api.js
```
## 実行結果
```vim

C:\Users\user\Documents\node.js_sample>node sample_api.js
[mocksrv] [req 0] [Sat, 29 Jan 2022 10:37:43 GMT] method: GET url: / req.body:
[mocksrv] [req 0] route for request not found
[mocksrv] [req 1] [Sat, 29 Jan 2022 10:37:53 GMT] method: GET url: /users req.body:
[mocksrv] [req 1] route for request not found
[mocksrv] [req 2] [Sat, 29 Jan 2022 10:38:33 GMT] method: GET url: /api req.body:
[mocksrv] [req 2] route for request not found
[mocksrv] [req 3] [Sat, 29 Jan 2022 10:39:49 GMT] method: GET url: /api/users req.body:
[mocksrv] [req 4] [Sat, 29 Jan 2022 10:40:35 GMT] method: GET url: /api/users req.body:
[mocksrv] [req 5] [Sat, 29 Jan 2022 10:40:35 GMT] method: GET url: /favicon.ico req.body:
[mocksrv] [req 5] route for request not found
[mocksrv] [req 6] [Sat, 29 Jan 2022 10:40:37 GMT] method: GET url: /api/users req.body:
・
・
・
```

## Powershellから以下実行

```vim
 curl http://localhost:4321/api/users
StatusCode        : 200
StatusDescription : OK
Content           : {91, 13, 10, 32...}
RawContent        : HTTP/1.1 200 OK
                    Connection: keep-alive
                    Keep-Alive: timeout=5
                    Transfer-Encoding: chunked
                    Date: Sat, 29 Jan 2022 10:39:49 GMT

                    [
                        {
                          'id': 1,
                          'name': 'John',
                          'mail': 'john@...
Headers           : {[Connection, keep-alive], [Keep-Alive, timeout=5], [Transfer-Encoding, chunked], [Date, Sat, 29 Jan 2022 10:39:4 
                    9 GMT]}
RawContentLength  : 179
```
## ブラウザから実行
![ブラウザ画面(Chrome)](/img/gamen2.png) 