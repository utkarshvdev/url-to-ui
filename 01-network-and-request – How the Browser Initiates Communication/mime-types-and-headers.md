# 🧾 3. MIME Types & HTTP Headers – Metadata & File Handling

## 🔸 Overview:

When a browser receives a response, it uses headers—especially MIME types—to decide how to interpret the body content. Headers also affect security and caching.

### 🧩 MIME Types (Multipurpose Internet Mail Extensions):

Define how the content should be handled.

Examples:

- text/html → render as HTML

- application/json → parse as JSON

- image/svg+xml → treat as SVG vector image

### 🧩 Important Headers:

- Content-Type: Declares MIME type

- X-Content-Type-Options: nosniff: Prevents content type guessing

- Access-Control-Allow-Origin: CORS policies

- Cache-Control: How the response should be cached

- Set-Cookie: Send a cookie to the browser

### 📌 Real Example:

```
Content-Type: application/json
Cache-Control: no-cache
Set-Cookie: sessionId=abc123; Secure; HttpOnly
```

### 🧠 Diagram:

```
| Header                   | Description                                    |
|--------------------------|------------------------------------------------|
| `Content-Type`           | Informs the browser of the media type (e.g., `text/css`) |
| `Cache-Control`          | Controls how long the content is cached (e.g., `max-age=31536000`) |
| `Set-Cookie`             | Sends cookies to the client (e.g., `token=xyz`) |
| `X-Content-Type-Options` | Prevents MIME type sniffing (`nosniff` improves security) |
```
