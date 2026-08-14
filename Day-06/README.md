# 📅 Day 06 — Web Fundamentals, Security & Cryptography

## 🎯 Today's Focus

Today I connected my networking knowledge with the Web, learned how websites communicate, understood the fundamental goals of cybersecurity, and started learning how cryptography protects information.

---

## 📚 Topics Completed

### 🌐 DNS
- Domain hierarchy
- TLD
- Second-Level Domain
- Subdomains
- A / AAAA Records
- CNAME
- MX
- TXT Records
- Recursive DNS
- Root DNS Servers
- TLD Servers
- Authoritative DNS Servers
- DNS Caching
- TTL

### 🌍 HTTP / HTTPS
- HTTP vs HTTPS
- URLs
- HTTP Requests
- HTTP Responses
- HTTP Methods
- HTTP Status Codes
- Request Headers
- Response Headers
- Cookies

### 🖥️ How Websites Work
- Web Servers
- Virtual Hosts
- Static Content
- Dynamic Content
- Frontend
- Backend
- Backend Languages

### 🏗️ Web Infrastructure
- Load Balancers
- CDN
- Databases
- WAF

### 🔺 CIA Triad
- Confidentiality
- Integrity
- Availability

### 🔐 Cryptography
- Plaintext
- Ciphertext
- Keys
- Algorithms
- Symmetric Encryption
- Caesar Cipher
- Key Distribution Problem
- Asymmetric Encryption
- Public Keys
- Private Keys
- Digital Certificates
- Certificate Authorities
- Hybrid Encryption

---

## 🧠 Main Concepts I Learned

### 🌐 DNS

Learned how DNS translates human-readable domain names into IP addresses and how different DNS servers work together to find the authoritative answer.

DNS allows us to communicate with internet services using names instead of remembering IP addresses.

A simplified flow:

Browser
   ↓
Local DNS Cache
   ↓
Recursive DNS Server
   ↓
Root DNS Server
   ↓
TLD Server
   ↓
Authoritative DNS Server
   ↓
IP Address


🌍 HTTP / HTTPS

Learned how browsers communicate with web servers using HTTP.

Browser
   │
   │ HTTP Request
   ▼
Web Server
   │
   │ HTTP Response
   ▼
Browser

I also learned common HTTP methods:

GET
POST
PUT
DELETE

And common status codes:

200 — OK
301 — Moved Permanently
302 — Found
400 — Bad Request
401 — Unauthorized
403 — Forbidden
404 — Not Found
500 — Internal Server Error
503 — Service Unavailable
📋 HTTP Headers

Learned that HTTP headers provide additional information about requests and responses.

Request Headers:

Host
User-Agent
Content-Length
Accept-Encoding
Cookie

Response Headers:

Set-Cookie
Cache-Control
Content-Type
Content-Encoding
🍪 Cookies

Learned how websites use cookies to remember information between requests.

Server
   ↓
Set-Cookie
   ↓
Browser stores cookie
   ↓
Browser sends Cookie
   ↓
Server recognizes session

This introduced an important concept that will become highly relevant when learning web application security.

🖥️ How Websites Work

Learned that a website is more than just a webpage sitting on a server.

A simplified architecture can look like:

User
 ↓
DNS
 ↓
Web Server
 ↓
Application / Backend
 ↓
Database

Additional infrastructure can include:

Load Balancers
CDN
WAF

Also learned the difference between static and dynamic content, and how frontend and backend components work together.

🔺 CIA Triad

Learned the three core principles cybersecurity aims to protect.

🔒 Confidentiality

Only authorized people should have access to information.

🧩 Integrity

Information should not be modified without authorization.

⚡ Availability

Systems and information should be accessible when authorized users need them.

🔐 Cryptography

Learned the basic structure of encryption:

Plaintext
    +
Encryption Algorithm
    +
Key
    ↓
Ciphertext

Decryption reverses the process.

🔑 Symmetric Encryption

Learned that symmetric encryption uses the same key for encryption and decryption.

        🔑 Same Secret Key
              │
              ▼
          Encryption
              │
              ▼
          Ciphertext
              │
              ▼
          Decryption
              │
              🔑
              ▼
           Plaintext

The major challenge is:

How can the secret key be shared securely?

This is known as the key distribution problem.

🔓 Asymmetric Encryption

Learned how asymmetric encryption uses two mathematically related keys:

🔓 Public Key
🔐 Private Key

For confidentiality:

Recipient Public Key
        ↓
     Encrypt
        ↓
   Ciphertext
        ↓
Recipient Private Key
        ↓
     Decrypt
        ↓
    Plaintext

This helps solve the key distribution problem because the public key can be shared openly.

📜 Certificates & Certificate Authorities

Learned that HTTPS uses digital certificates to associate a public key with a website's identity.

Certificate Authorities (CAs) help establish trust by digitally signing certificates.

Browsers can check information such as:

Certificate issuer
Validity
Expiration
Domain association
🔄 Hybrid Encryption

One of the most important concepts from today's learning was how modern secure communication combines asymmetric and symmetric encryption.

             HTTPS
               │
               ▼
      Asymmetric Cryptography
               │
               │ Establish / exchange keys
               ▼
       Shared Symmetric Key
               │
               ▼
       Symmetric Encryption
               │
               ▼
        Fast Data Transfer

Asymmetric encryption:

Helps with secure key establishment and trust.

Symmetric encryption:

Is fast and efficient for encrypting large amounts of data.

🎯 Today's Key Takeaway

I now understand the basic journey of a web request — from DNS resolution to HTTP communication and web infrastructure — and how cybersecurity principles and cryptography are used to protect the systems and data involved.

The biggest cryptography concept I understood today:

Symmetric encryption is fast but has a key-distribution problem. Asymmetric encryption helps solve that problem, while modern secure communication combines both approaches.

📈 Pre Security Progress
Introduction to Cyber Security ✅
Computer Fundamentals ✅
Operating Systems Basics ✅
Software Basics ✅
Network Fundamentals ✅
Web Fundamentals ✅
CIA Triad ✅
Cryptography Concepts ✅
🔥 Grinding Status

Day 06 — COMPLETE ✅

6 days of consistent cybersecurity learning.
