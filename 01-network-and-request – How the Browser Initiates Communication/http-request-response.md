## 📡 2. HTTP Request & Response – Communicating with the Server


## 🧩 Request Lifecycle:

(i) - Request: GET /index.html HTTP/1.1

(ii) - Headers: Metadata like User-Agent, Accept, Cookie

(iii) - Body (optional): Only in POST/PUT

```
GET /index.html HTTP/1.1
Host: example.com
User-Agent: Mozilla/5.0
Accept: text/html
```


## 🧩 Response Lifecycle:

(i) - Status: HTTP/1.1 200 OK

(ii) - Headers: Content-Type, Set-Cookie, Cache-Control

(iii) - Body: Actual HTML, JSON, image, etc.

```
HTTP/1.1 200 OK
Content-Type: text/html
Set-Cookie: theme=dark; Path=/

<html>...</html>
```

## 📌 Connection Reuse:

HTTP/1.1 supports Keep-Alive by default.

Modern HTTP/2 and HTTP/3 multiplex requests and improve performance.

```
[Browser] ⇄ [Server]
   ⇢ GET /index.html
   ⇠ 200 OK + HTML
```
