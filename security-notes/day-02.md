# Day 02 — OSI Model

The **OSI (Open Systems Interconnection) Model** is a 7-layer framework used to understand how devices communicate across a network.

For cybersecurity, the OSI model helps identify **where network activity and attacks occur**.

| Layer                | What it does                                                      | Data Unit          | Example Device | Example Attack    |
| -------------------- | ----------------------------------------------------------------- | ------------------ | -------------- | ----------------- |
| **7 — Application**  | Provides network services directly to applications and users.     | Data               | Proxy / WAF    | SQL Injection     |
| **6 — Presentation** | Handles data formatting, encoding, encryption and compression.    | Data               | Gateway        | TLS/SSL attacks   |
| **5 — Session**      | Establishes, manages and terminates communication sessions.       | Data               | Gateway        | Session hijacking |
| **4 — Transport**    | Provides end-to-end communication using TCP or UDP.               | Segment / Datagram | Firewall       | SYN flood         |
| **3 — Network**      | Handles logical addressing and routing between networks.          | Packet             | Router         | IP spoofing       |
| **2 — Data Link**    | Handles local network delivery using MAC addresses.               | Frame              | Switch         | ARP spoofing      |
| **1 — Physical**     | Transmits raw bits through cables, radio or other physical media. | Bits               | Hub            | Cable tapping     |

## Security Perspective

A useful way to remember the model:

**7 — Application** → What the application is doing
**6 — Presentation** → How the data is represented/protected
**5 — Session** → How communication sessions are maintained
**4 — Transport** → How data gets delivered end-to-end
**3 — Network** → Where the data should go
**2 — Data Link** → How devices communicate on the local network
**1 — Physical** → How the bits physically travel

## Key Security Takeaway

The OSI model isn't just a networking theory tool. It can help a security analyst answer:

> **"At which layer is this activity happening, and what security controls or attacks are relevant there?"**

For example:

* **ARP spoofing → Layer 2**
* **IP spoofing → Layer 3**
* **SYN flooding → Layer 4**
* **SQL injection → Layer 7**

## Lab

Tools used:

* Wireshark
* Linux terminal
* Git/GitHub

