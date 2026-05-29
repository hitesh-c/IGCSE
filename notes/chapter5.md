# Chapter 5 — The Internet and its Uses (Short Notes

**Cambridge IGCSE & O Level Computer Science** · Quick revision notes
Sections: **5.1** Internet & WWW · **5.2** Digital currency · **5.3** Cyber security

---

# 5.1 The internet and the World Wide Web (WWW)

## 5.1.1 Internet vs WWW

| Internet | World Wide Web (WWW) |
|---|---|
| Worldwide collection of interconnected **networks and devices**. | A collection of **multimedia web pages** on websites. |
| A **concept** relying on physical infrastructure. | Accessed using a **web browser**; based on http(s). |
| Uses **TCP/IP** protocols; lets you send email and chat. | Uses **URLs** to locate web pages; pages written in **HTML**. |

The WWW is **part of** the internet — a way of accessing information using the internet.

## 5.1.2 Uniform Resource Locators (URLs)

A URL is a text address for a web page. Format:
`protocol://website address/path/file name`

- **Protocol** — `http` or `https`.
- **Website address** — domain host (`www`), domain name, domain type (`.com`, `.org`, `.gov`), sometimes country code (`.uk`, `.de`).
- **Path** — the web page (if omitted, defaults to the root directory).
- **File name** — the item on the web page.

Example: `https://www.hoddereducation.co.uk/ict`

## 5.1.3 HTTP and HTTPS

- **HTTP** (Hypertext Transfer Protocol) — rules for transferring files across the internet.
- **HTTPS** — HTTP with security applied (SSL/TLS). The **'s' = secure**; shown by a **green padlock** in the address bar.

## 5.1.4 Web browsers

Software that accesses web pages and **interprets HTML** to display text, images, video and audio. Common features:

- Has a **home page**; stores **bookmarks** (favourites) and **user history**.
- Navigate **forwards/backwards**; open **multiple tabs**.
- Uses **cookies**, stores data in a **cache**, runs **JavaScript**.
- Uses **hyperlinks** (open in new tab with Ctrl+click, or same tab by clicking).
- Has an **address bar**.

## 5.1.5 Location and retrieval of web pages (DNS)

Websites are written in **HTML** and hosted on a web server with its own **IP address**. The **Domain Name Server (DNS)** converts a URL into an IP address. Process:

1. User types the URL; browser asks **DNS server 1** for the IP address.
2. If DNS server 1 can't find it, it requests **DNS server 2**.
3. DNS server 2 maps the URL to its IP address and returns it; DNS server 1 stores it in its cache.
4. The IP address is sent back to the user's computer.
5. The computer connects to the website server; **HTML files** are sent back and the browser displays the page.

## 5.1.6 Cookies

Small files/code sent by a web server and stored on the user's computer. Each is a small look-up table of **(key, data)** pairs. They enable **user tracking** and store **user preferences**.

| Session cookie | Persistent (permanent) cookie |
|---|---|
| Stored in **temporary memory**. | Stored on the **hard drive**. |
| **Deleted** when the browser/session closes. | Remains until the **expiry date** or the user deletes it. |
| Used to hold items in a **virtual shopping basket**; does not identify the user. | Remembers **login details**, preferences; removes need to re-enter data. |
| No expiry date = always a session cookie. | Personal data in it should be **encrypted**. |

**Uses of (persistent) cookies:** remember passwords/emails/invoice details; recognise returning users; save items in a basket; track internet habits; targeted advertising; store preferences and language; online transactions; save game progress.

---

# 5.2 Digital currency

## 5.2.1 What is digital currency?

- Money that exists **only in digital form** (no physical form), unlike **fiat currency** ($, £, €) which is backed by governments/banks.
- Accepted as payment and transferable between accounts (e.g. PayPal, Apple Pay).
- Relies on a **central banking system** → problem: maintaining **confidentiality and security** (centralisation).

**Cryptocurrency** solves this with **decentralisation**:

- Uses **cryptography** to track transactions.
- Has **no state control** — rules set by the community.
- Transactions are **publicly available** and trackable.
- Works within a **blockchain network**, making it more secure.

## 5.2.2 Blockchaining

A **decentralised database** of all transactions, held on many interconnected computers with **no central server**. Every networked computer gets a copy of each transaction, so it **cannot be changed without consent** of all members.

**Each block contains:**

- **Data** — e.g. sender, recipient, amount.
- **Hash value** — a unique "fingerprint" from an algorithm (often SHA-256), including a **timestamp**.
- **Previous hash value** — points back to the previous block.

**How it stays secure:**

- The first block is the **genesis block** (no previous block).
- Changing a block changes its hash → breaks the chain → all later blocks become **invalid** → tampering is detected.
- **Proof-of-work** makes creating each block take ~10 minutes, slowing down attackers.
- **Miners** (special users) verify transactions and create blocks for a reward.
- Almost impossible to hack — every block would need attacking at the same time.

**Uses:** cryptocurrency exchanges, smart contracts, research, politics, education.

---

# 5.3 Cyber security

## 5.3.1 Cyber security threats

**Brute force attack** — systematically trying all combinations of characters to crack a password. Sped up with **common-password lists** and **word lists**. Longer, varied passwords are harder to crack.

**Data interception** — stealing data from a wired/wireless link:
- **Packet sniffer** — examines data packets (common on wired networks).
- **Wardriving** (Access Point Mapping) — intercepts Wi-Fi using a laptop/phone, antenna and GPS.
- Defend with **encryption**, **WEP protocol**, a **firewall**, complex router passwords; avoid public Wi-Fi.

**Distributed Denial of Service (DDoS)** — flooding a server/mailbox with **fake requests/spam** from **many computers** so legitimate users are denied access. Signs: slow performance, can't access sites, lots of spam. Defend with malware checkers, **firewalls**, **email filters**.

**Hacking** — gaining **illegal access** to a system; can delete/corrupt/steal data. Encryption makes data meaningless but doesn't stop hacking. Defend with firewalls, strong passwords, anti-hacking/intrusion-detection software. **Ethical hacking** = authorised paid hackers testing security.

**Malware** — six main types:

| Type | Description |
|---|---|
| **Virus** | Replicates to delete/corrupt files; needs an **active host** to run. |
| **Worm** | Stand-alone, self-replicating; spreads through networks **without user action**; no host needed. |
| **Trojan horse** | Disguised as legitimate software; must be **run by the user**; often delivers spyware/ransomware. |
| **Spyware** | Monitors activity and sends data back to the criminal; **key-logging** captures key presses. |
| **Adware** | Floods the user with **unwanted advertising**/pop-ups; can hijack the browser. |
| **Ransomware** | **Encrypts** data and holds it hostage until a **ransom** is paid; defend with **back-ups**. |

**Phishing** — legitimate-looking **emails** with links/attachments that lead to a fake site or trick the user into giving data. The user **must act** for it to work. **Spear phishing** targets specific people/companies. Defend: don't click unknown links, anti-phishing toolbars, look for https/padlock, up-to-date browser and firewall.

**Pharming** — malicious code redirects the browser to a **fake website** with **no user action** (e.g. via **DNS cache poisoning**, which changes IP addresses on the DNS). Defend: anti-virus, modern browsers, check spelling, https/padlock.

**Social engineering** — manipulating people into breaking security procedures. Five types: **instant messaging**, **phishing emails**, **baiting** (infected memory stick left to be found), **phone calls**, **scareware** (fake anti-virus pop-up). Exploits three emotions: **fear, curiosity, empathy/trust**. Four stages: (1) identify victim, (2) target, (3) execute attack, (4) cover tracks.

## 5.3.2 Keeping data safe

**Access levels** — a hierarchy of rights via user name/password (e.g. hospital consultant vs cleaner). Social networks use **four levels**: public, friends, custom, data owner — controlled by **privacy settings**.

**Anti-malware** — **anti-virus** (see Chapter 4) and **anti-spyware** (detects spyware using **rules** or **file structures**). Anti-spyware also: prevents downloads, encrypts files and keystrokes, blocks webcam/microphone access, scans for stolen data.

**Authentication** — proving identity using:
- **Something you know** (password/PIN)
- **Something you have** (phone/tablet)
- **Something unique to you** (biometrics)

**Passwords** — restrict access; should be **strong** and changed regularly. A **strong password** has at least one capital, one number, one special character (e.g. `Sy12@#TT90kj=0`); a **weak** one is short/predictable (e.g. `GREEN`). Protect with anti-spyware; limited login attempts (usually 3) then lockout; reset via email link.

**Biometrics** — uses unique human characteristics:

| Technique | Benefits | Drawbacks |
|---|---|---|
| **Fingerprint** | Well developed, easy, small storage. | Intrusive for some; fails with dirty/damaged skin. |
| **Retina** | Very high accuracy; cannot be replicated. | Intrusive, slow, expensive. |
| **Face recognition** | Non-intrusive, inexpensive. | Affected by lighting, hair, ageing, glasses. |
| **Voice recognition** | Non-intrusive, fast (<5s), inexpensive. | Voice can be recorded; low accuracy; illness changes voice. |

*Example application:* retina scanner → ADC → microprocessor compares with database → match unlocks the door via a DAC and actuator (light turns green).

**Two-step verification** — two methods of authentication, e.g. password (**something you know**) **plus** a **one-time pass code** texted to a registered phone (**something you have**).

**Automatic software updates** — keep software current; deliver **patches** that fix security holes, remove bugs, add features.

**Checking emails/URLs** — before opening, check **spelling, tone and links**. Watch for: wrong email domain after `@`, urgent/threatening tone, bad spelling, **typo squatting** (e.g. `gougle.com`, `amozon.com`), suspicious hover-link destinations, missing https.

**Firewalls** — software or hardware sitting between the computer and an external network; filters incoming/outgoing traffic. Tasks: examine traffic against criteria, block/log/warn, block undesirable IP addresses, warn when software accesses external sources. **Limitations:** can't stop users' own devices bypassing it, employee misconduct, or a user disabling it.

**Proxy servers** — act as an **intermediary** between user and web server. Filter traffic, hide the user's IP, block invalid requests/IPs, take the hit in an attack (protect against DoS/hacking), and use a **cache** to speed up page access. Can also act as a firewall.

**Privacy settings** — controls limiting who sees a profile: "do not track", saved-payment checks, safe browsing alerts (blacklist), cookie/history options, advertising opt-outs, app location sharing.

**Secure Sockets Layer (SSL)** — a protocol that **encrypts** data sent over the internet so only the user's computer and server can read it (shown by https/padlock). Uses an **SSL certificate** (a digital certificate) to **authenticate** a website. SSL handshake:

1. Browser requests the web server identify itself.
2. Server sends a copy of its **SSL certificate**.
3. Browser authenticates the certificate and replies.
4. Server acknowledges; **encrypted two-way transfer begins**.

Used for: online banking/shopping, email, cloud storage, intranets/extranets, VoIP, instant messaging, social networks.

> **Extension — TLS:** Transport Layer Security is a newer, more secure version of SSL providing encryption, authentication and data integrity. It has two layers: **record protocol** (holds the data) and **handshake protocol** (authentication + encryption). TLS supports new authentication methods and **session caching** to improve performance.

---

# Key terms (quick glossary)

| Term | Meaning |
|---|---|
| **Internet** | Worldwide interconnection of networks using TCP/IP. |
| **WWW** | Collection of web pages based on http(s). |
| **Web browser** | Software that locates IP addresses (via DNS) and interprets HTML. |
| **HTML** | Language used to design and display web pages. |
| **URL** | Text-based address of a web page. |
| **HTTPS** | HTTP with extra security (SSL/TLS). |
| **Hyperlink** | Clickable text/image linking to other content. |
| **DNS** | Server that maps domain names to IP addresses. |
| **Cookie** | Text file remembering user preferences. |
| **Session cookie** | Temporary cookie deleted when the browser closes. |
| **Persistent cookie** | Cookie stored on the hard drive until expiry/deletion. |
| **Digital currency** | Money existing in electronic form only. |
| **Cryptocurrency** | Decentralised digital currency tracked by a chain of computers. |
| **Cryptography** | Protecting data using encryption/decryption. |
| **Blockchain** | Decentralised database of transactions across many computers. |
| **Timestamp** | Record of when a block was created. |
| **Proof-of-work** | Algorithm that confirms a transaction and creates new blocks. |
| **Brute force attack** | Trial-and-error cracking of passwords. |
| **Word list** | Text file of words used in a brute force attack. |
| **Data interception** | Eavesdropping on a network transmission. |
| **Packet sniffing** | Examining data packets sent over a network. |
| **Wardriving** | Intercepting Wi-Fi signals to steal data. |
| **WEP** | Wireless encryption protocol protecting against interception. |
| **DoS / DDoS attack** | Flooding a server with requests to deny service (DDoS = from many computers). |
| **Spam** | Unsolicited emails. |
| **Hacking** | Gaining illegal access to a computer system. |
| **Malware** | Programs that delete, corrupt or manipulate data illegally. |
| **Virus** | Self-replicating code needing an active host. |
| **Active host** | Software a virus attaches to in order to run. |
| **Worm** | Stand-alone self-replicating malware needing no host. |
| **Trojan horse** | Malware disguised as legitimate software. |
| **Spyware** | Malware that monitors activity and reports back. |
| **Adware** | Malware that floods the user with advertising. |
| **Ransomware** | Malware that encrypts data until a ransom is paid. |
| **Phishing** | Fake emails tricking users into giving personal data. |
| **Spear phishing** | Phishing aimed at specific people/organisations. |
| **Pharming** | Redirecting a user to a fake website without their action. |
| **DNS cache poisoning** | Altering DNS IP addresses to redirect users to fake sites. |
| **Social engineering** | Manipulating people into breaking security procedures. |
| **Access levels** | Hierarchy of access rights based on user security level. |
| **Anti-spyware** | Software that detects/removes spyware using rules or file structures. |
| **Authentication** | Proving identity (know / have / unique to you). |
| **Biometrics** | Authentication using unique human characteristics. |
| **Two-step verification** | Authentication using two methods. |
| **Patch** | Software update that fixes bugs/security. |
| **Typo squatting** | Using misspelt website addresses to fool users. |
| **Firewall** | Software/hardware filtering traffic between a computer and a network. |
| **Proxy server** | Intermediary server that filters requests and caches pages. |
| **Privacy settings** | Controls limiting who can access a user's profile. |
| **SSL** | Security protocol for sending data over a network. |
| **SSL certificate** | Digital certificate used to authenticate a website. |

---

# Quick check questions

1. State three differences between the internet and the WWW.
2. Identify each part of the URL `https://www.example.co.uk/page`.
3. Outline the DNS process used to retrieve a web page.
4. Give two differences between session and persistent cookies.
5. Explain how a blockchain prevents a transaction from being tampered with.
6. Describe how a DDoS attack works and two ways to defend against it.
7. Name the six types of malware and state one feature of each.
8. Explain the difference between phishing and pharming.
9. List the three factors of authentication, with an example of each.
10. Compare fingerprint and retina scanning as biometric methods.
11. Describe how SSL provides a secure connection between a browser and a website.
