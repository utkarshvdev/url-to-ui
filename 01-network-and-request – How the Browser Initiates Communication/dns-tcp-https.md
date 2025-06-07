🌐 1. DNS → TCP → HTTPS – From URL to Connection

🔸 Overview:

When a user types a URL like https://example.com into the browser, several network-level operations occur before the browser even requests the content. This section dives deep into that journey.

🧩 Step-by-Step Breakdown:

1. DNS Resolution (Domain to IP)

The browser checks the local cache → OS cache → router cache → ISP DNS cache → authoritative DNS servers.

A recursive DNS resolver is used to find the actual IP.

Uses UDP on port 53.

🔧 Tool Tip: Try nslookup example.com or dig example.com to see DNS in action.

example.com
   ↓
93.184.216.34 (IP Address)


2. TCP Handshake (3-Way Connection Setup)

Occurs on port 80 (HTTP) or 443 (HTTPS).

Ensures reliable transmission using:

SYN → Client initiates

SYN-ACK → Server acknowledges

ACK → Client confirms

Client: SYN ➝
Server:    ⇠ SYN-ACK
Client: ➝ ACK


This handshake establishes a socket (connection ID) between client and server.

3. TLS Handshake (Secure the Channel)

Starts with ClientHello: Cipher suites, TLS version, and random number.

ServerHello: Chosen cipher, certificate.

Certificate is verified using CA (Certificate Authority).

Pre-master secret is exchanged (via RSA or Diffie-Hellman), used to derive session keys.

ClientHello → ServerHello
      ↓               ↓
  Certificate     Session Keys
      ↓               ↓
   Encrypted channel is established (HTTPS)


🔐 Once secure, HTTP can begin on top of this encrypted TCP connection.

✅ Key Takeaways:

DNS translates names to IPs.

TCP ensures ordered delivery.

TLS protects confidentiality and authenticity.