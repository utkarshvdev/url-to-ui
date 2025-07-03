# 🌐 DNS, TCP, and HTTPS – The First Steps of Loading a Web Page


### 🔹 1. What Happens When You Enter a URL?


When you type a URL like `https://github.com`, the browser doesn't directly know the IP address of the server. It needs to:


1. **Resolve the domain** (DNS)
2. **Establish a connection** (TCP)
3. **Secure the connection** (TLS/HTTPS)
4. Then send the HTTP request

---


### 🧭 2. DNS (Domain Name System)

- Maps human-readable domains to IP addresses.
- Uses recursive resolvers, root servers, TLD servers, and authoritative name servers.
- DNS result may be cached:
  - In your OS (e.g., `/etc/hosts`)
  - By the browser
  - By your ISP's DNS server

```
**Example:**  
`github.com` ➝ `140.82.121.3`
```

---

### 🔗 3. TCP (Transmission Control Protocol)

- A reliable transport protocol (3-way handshake)
- Steps:
  1. Client: SYN
  2. Server: SYN-ACK
  3. Client: ACK
- Now the connection is "established" — and data can flow.

---

### 🔐 4. HTTPS (TLS/SSL Layer)

- HTTPS = HTTP over TLS (formerly SSL)
- Ensures data is:
  - **Encrypted**
  - **Authenticated**
  - **Integrity-checked**

**TLS Handshake Involves:**
- Server certificate verification
- Exchange of encryption keys
- Agreed-upon cipher suites

---

### 📌 Summary Flow

```text
URL ➝ DNS ➝ IP ➝ TCP ➝ TLS ➝ Secure Connection Ready
