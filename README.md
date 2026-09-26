# Web-Security Papers — Offensive & Defensive

**131 peer-reviewed web-security & web-privacy papers** (70 offensive, 61 defensive), 277.5 MB total,
split into two collections under `papers/` and categorized into topic subdirectories by reading each paper's abstract.

- **`papers/Offensive-Papers/`** — 70 papers across 12 topics: attacks, exploitation, vulnerability discovery, and offensive measurement.
- **`papers/Defensive-Papers/`** — 61 papers across 11 topics: detection, mitigation, hardening, and privacy/compliance.

Sourced from three open-access venues — **NDSS**, **USENIX Security**, and **PoPETs (PETS)** — editions **2024, 2025, 2026**.
Of these, 73 were in the original 2025–2026 set and **58 were newly added** (2024 editions + 2025–2026 gaps).

## How papers are classified

Each paper is placed by the **core contribution of the work**, decided from its abstract:

- **Offensive** — a new attack/exploit, vulnerability-discovery tooling (fuzzers, taint analysis, scanners, exploit synthesis, gadget mining), a new tracking/fingerprinting technique, or a measurement that *exposes* a weakness or user surveillance.
- **Defensive** — detection of attacks at runtime, mitigation/hardening, anti-tracking or privacy-preserving mechanisms, compliance/consent enforcement, phishing/scam detectors, or a defensive SoK/benchmark.

Borderline privacy work uses a consistent tie-breaker: a reusable **detector/defense** → Defensive; a **measurement/audit that exposes tracking** → Offensive; **consent/opt-out compliance** studies → Defensive.

## Directory layout

```
papers/
  Offensive-Papers/
    Tracking-and-Fingerprinting/
    HTTP-Protocol-and-Transport-Attacks/
    Web-App-Vulnerability-Discovery-and-Scanning/
    Authentication-Identity-and-Access-Attacks/
    Injection-Taint-and-Deserialization/
    Phishing-Scams-and-Web-Abuse/
    Runtime-Engine-and-Browser-Internals/
    XSS-and-DOM/
    DoS-and-Availability/
    Domain-and-DNS-Takeover/
    Payment-and-Authorization-Attacks/
    Web-Agent-and-LLM-Attacks/
  Defensive-Papers/
    Anti-Tracking-and-Privacy-Defenses/
    Phishing-and-Scam-Detection/
    Privacy-Compliance-and-Consent/
    Authentication-and-Passkey-Defenses/
    PKI-and-Transport-Security/
    Vulnerability-Mitigation-and-Hardening/
    Web-Attack-and-Malware-Detection/
    Web-Agent-and-LLM-Security/
    Measurement-Tools-and-SoK/
    Supply-Chain-Security/
    Content-Protection-and-Anti-Crawling/
```

## Coverage by venue

| Venue | Papers |
|---|---|
| NDSS 2024 | 10 |
| NDSS 2025 | 11 |
| NDSS 2026 | 13 |
| PoPETs 2024 | 12 |
| PoPETs 2025 | 8 |
| PoPETs 2026 | 8 |
| USENIX-Security 2024 | 25 |
| USENIX-Security 2025 | 24 |
| USENIX-Security 2026 | 20 |

## Files

- `papers_index.csv` — one row per paper: side, topic, venue, year, title, verdict, PDF URL, local path, size.
- `validation.csv` — per-paper extracted abstract and web-relevance evidence.

---

## Offensive-Papers (70)

New attacks, exploitation, vulnerability discovery, and offensive measurements that expose weaknesses or user surveillance.

### Tracking and Fingerprinting (14)
_Browser/mobile fingerprinting and tracking techniques and measurements that expose user surveillance._

- **Untangle Multi-Layer Web Server Fingerprinting** (NDSS 2024)  
  [PDF](https://www.ndss-symposium.org/wp-content/uploads/2024-497-paper.pdf) · `papers/Offensive-Papers/Tracking-and-Fingerprinting/NDSS-2024__Untangle-Multi-Layer-Web-Server-Fingerprinting.pdf`
- **Cascading Spy Sheets Exploiting The Complexity Of Modern Css For Email And Browser Fingerprinting** (NDSS 2025)  
  [PDF](https://www.ndss-symposium.org/wp-content/uploads/2025-s238-paper.pdf) · `papers/Offensive-Papers/Tracking-and-Fingerprinting/NDSS-2025__Cascading-Spy-Sheets-Exploiting-The-Complexity-Of-Modern-Css-For-Email-And-Browser-Fingerprinti.pdf`
- **Cross Boundary Mobile Tracking Exploring Java To Javascript Information Diffusion In Webviews** (NDSS 2026)  
  [PDF](https://www.ndss-symposium.org/wp-content/uploads/2026-s910-paper.pdf) · `papers/Offensive-Papers/Tracking-and-Fingerprinting/NDSS-2026__Cross-Boundary-Mobile-Tracking-Exploring-Java-To-Javascript-Information-Diffusion-In-Webviews.pdf`
- **How Unique is Whose Web Browser? The role of demographics in browser fingerprinting among US users** (PoPETs 2025)  
  [PDF](https://petsymposium.org/popets/2025/popets-2025-0038.pdf) · `papers/Offensive-Papers/Tracking-and-Fingerprinting/PoPETs-2025__How-Unique-is-Whose-Web-Browser-The-role-of-demographics-in-browser-fingerprinting-among-US-use.pdf`
- **Intractable Cookie Crumbs: Unveiling the Nexus of Stateful Banner Interaction and Tracking Cookies** (PoPETs 2025)  
  [PDF](https://petsymposium.org/popets/2025/popets-2025-0138.pdf) · `papers/Offensive-Papers/Tracking-and-Fingerprinting/PoPETs-2025__Intractable-Cookie-Crumbs-Unveiling-the-Nexus-of-Stateful-Banner-Interaction-and-Tracking-Cooki.pdf`
- **Tracking Without Borders: Studying the Role of WebViews in Bridging Mobile and Web Tracking** (PoPETs 2025)  
  [PDF](https://petsymposium.org/popets/2025/popets-2025-0155.pdf) · `papers/Offensive-Papers/Tracking-and-Fingerprinting/PoPETs-2025__Tracking-Without-Borders-Studying-the-Role-of-WebViews-in-Bridging-Mobile-and-Web-Tracking.pdf`
- **Clicking into Exposure: Uncovering Privacy Risks of Google Click Identifier in YouTube Ads** (PoPETs 2026)  
  [PDF](https://petsymposium.org/popets/2026/popets-2026-0038.pdf) · `papers/Offensive-Papers/Tracking-and-Fingerprinting/PoPETs-2026__Clicking-into-Exposure-Uncovering-Privacy-Risks-of-Google-Click-Identifier-in-YouTube-Ads.pdf`
- **The Empire Strikes Back (at Your Privacy): An Archaeology of Tracking on Government Websites** (PoPETs 2026)  
  [PDF](https://petsymposium.org/popets/2026/popets-2026-0039.pdf) · `papers/Offensive-Papers/Tracking-and-Fingerprinting/PoPETs-2026__The-Empire-Strikes-Back-at-Your-Privacy-An-Archaeology-of-Tracking-on-Government-Websites.pdf`
- **The Masks We (Think We) Wear: Privacy Threats of Browser-Extension Wallets in the Web3 Ecosystem** (PoPETs 2026)  
  [PDF](https://petsymposium.org/popets/2026/popets-2026-0094.pdf) · `papers/Offensive-Papers/Tracking-and-Fingerprinting/PoPETs-2026__The-Masks-We-Think-We-Wear-Privacy-Threats-of-Browser-Extension-Wallets-in-the-Web3-Ecosystem.pdf`
- **Smudged Fingerprints Characterizing and Improving the Performance of Web Application Fingerprinting** (USENIX-Security 2024)  
  [PDF](https://www.usenix.org/system/files/usenixsecurity24-kondracki.pdf) · `papers/Offensive-Papers/Tracking-and-Fingerprinting/USENIX-Security-2024__Smudged-Fingerprints-Characterizing-and-Improving-the-Performance-of-Web-Application-Finge.pdf`
- **Big Help or Big Brother Auditing Tracking Profiling and Personalization in Generative AI Assistants** (USENIX-Security 2025)  
  [PDF](https://www.usenix.org/system/files/usenixsecurity25-vekaria.pdf) · `papers/Offensive-Papers/Tracking-and-Fingerprinting/USENIX-Security-2025__Big-Help-or-Big-Brother-Auditing-Tracking-Profiling-and-Personalization-in-Generative-AI-A.pdf`
- **Double-Edged Shield: On the Fingerprintability of Customized Ad Blockers** (USENIX-Security 2025)  
  [PDF](https://www.usenix.org/system/files/usenixsecurity25-el-hajj-chehade.pdf) · `papers/Offensive-Papers/Tracking-and-Fingerprinting/USENIX-Security-2025__Double-Edged-Shield-On-the-Fingerprintability-of-Customized-Ad-Blockers.pdf`
- **HyTrack: Resurrectable and Persistent Tracking Across Android Apps and the Web** (USENIX-Security 2025)  
  [PDF](https://www.usenix.org/system/files/usenixsecurity25-wessels.pdf) · `papers/Offensive-Papers/Tracking-and-Fingerprinting/USENIX-Security-2025__HyTrack-Resurrectable-and-Persistent-Tracking-Across-Android-Apps-and-the-Web.pdf`
- **Bridges to Self: Silent Web-to-App Tracking on Mobile via Localhost** (USENIX-Security 2026)  
  [PDF](https://www.usenix.org/system/files/usenixsecurity26-vlummens.pdf) · `papers/Offensive-Papers/Tracking-and-Fingerprinting/USENIX-Security-2026__Bridges-to-Self-Silent-Web-to-App-Tracking-on-Mobile-via-Localhost.pdf`

### HTTP Protocol and Transport Attacks (9)
_HTTP/2-3 issues, request smuggling/desync, CDN translation anomalies, WebRTC, and TLS-layer attacks on web servers._

- **ReqsMiner Automated Discovery of CDN Forwarding Request Inconsistencies and DoS Attacks with Grammar-based Fuzzing** (NDSS 2024)  
  [PDF](https://www.ndss-symposium.org/wp-content/uploads/2024-31-paper.pdf) · `papers/Offensive-Papers/HTTP-Protocol-and-Transport-Attacks/NDSS-2024__Reqsminer-Automated-Discovery-Of-Cdn-Forwarding-Request-Inconsistencies-And-Dos-Attacks-Wi.pdf`
- **Cross Origin Web Attacks Via Http 2 Server Push And Signed Http Exchange** (NDSS 2025)  
  [PDF](https://www.ndss-symposium.org/wp-content/uploads/2025-1086-paper.pdf) · `papers/Offensive-Papers/HTTP-Protocol-and-Transport-Attacks/NDSS-2025__Cross-Origin-Web-Attacks-Via-Http-2-Server-Push-And-Signed-Http-Exchange.pdf`
- **Racing for TLS Certificate Validation A Hijacker's Guide to the Android TLS Galaxy** (USENIX-Security 2024)  
  [PDF](https://www.usenix.org/system/files/usenixsecurity24-pourali.pdf) · `papers/Offensive-Papers/HTTP-Protocol-and-Transport-Attacks/USENIX-Security-2024__Racing-for-TLS-Certificate-Validation-A-Hijacker-s-Guide-to-the-Android-TLS-Galaxy.pdf`
- **STEK Sharing is Not Caring: Bypassing TLS Authentication in Web Servers using Session Tickets** (USENIX-Security 2025)  
  [PDF](https://www.usenix.org/system/files/usenixsecurity25-hebrok.pdf) · `papers/Offensive-Papers/HTTP-Protocol-and-Transport-Attacks/USENIX-Security-2025__STEK-Sharing-is-Not-Caring-Bypassing-TLS-Authentication-in-Web-Servers-using-Session-Tickets.pdf`
- **The Silent Danger in HTTP: Identifying HTTP Desync Vulnerabilities with Gray-box Testing** (USENIX-Security 2025)  
  [PDF](https://www.usenix.org/system/files/usenixsecurity25-mu.pdf) · `papers/Offensive-Papers/HTTP-Protocol-and-Transport-Attacks/USENIX-Security-2025__The-Silent-Danger-in-HTTP-Identifying-HTTP-Desync-Vulnerabilities-with-Gray-box-Testing.pdf`
- **Analyzing the WebRTC Ecosystem and Breaking Authentication in DTLS-SRTP** (USENIX-Security 2026)  
  [PDF](https://www.usenix.org/system/files/usenixsecurity26-bach.pdf) · `papers/Offensive-Papers/HTTP-Protocol-and-Transport-Attacks/USENIX-Security-2026__Analyzing-the-WebRTC-Ecosystem-and-Breaking-Authentication-in-DTLS-SRTP.pdf`
- **H3Act: Automated Measuring Semantic Conversion Anomalies of HTTP/3-to-HTTP/1.1 Translation in CDNs** (USENIX-Security 2026)  
  [PDF](https://www.usenix.org/system/files/usenixsecurity26-peng-qihang.pdf) · `papers/Offensive-Papers/HTTP-Protocol-and-Transport-Attacks/USENIX-Security-2026__H3Act-Automated-Measuring-Semantic-Conversion-Anomalies-of-HTTP-3-to-HTTP-1-1-Translation-in-CD.pdf`
- **Opossum Attack: Application Layer Desynchronization using Opportunistic TLS** (USENIX-Security 2026)  
  [PDF](https://www.usenix.org/system/files/usenixsecurity26-merget.pdf) · `papers/Offensive-Papers/HTTP-Protocol-and-Transport-Attacks/USENIX-Security-2026__Opossum-Attack-Application-Layer-Desynchronization-using-Opportunistic-TLS.pdf`
- **Plain Text, Plain Risks: Measuring HTTP Inclusion in Android WebViews at Scale** (USENIX-Security 2026)  
  [PDF](https://www.usenix.org/system/files/usenixsecurity26-beer.pdf) · `papers/Offensive-Papers/HTTP-Protocol-and-Transport-Attacks/USENIX-Security-2026__Plain-Text-Plain-Risks-Measuring-HTTP-Inclusion-in-Android-WebViews-at-Scale.pdf`

### Web App Vulnerability Discovery and Scanning (9)
_Black/grey-box scanners, crawlers, and fuzzers that find server-side and web-application vulnerabilities._

- **Compromising Industrial Processes using Web-Based Programmable Logic Controller Malware** (NDSS 2024)  
  [PDF](https://www.ndss-symposium.org/wp-content/uploads/2024-49-paper.pdf) · `papers/Offensive-Papers/Web-App-Vulnerability-Discovery-and-Scanning/NDSS-2024__Compromising-Industrial-Processes-Using-Web-Based-Programmable-Logic-Controller-Malware.pdf`
- **Eagleye Exposing Hidden Web Interfaces In Iot Devices Via Routing Analysis** (NDSS 2025)  
  [PDF](https://www.ndss-symposium.org/wp-content/uploads/2025-399-paper.pdf) · `papers/Offensive-Papers/Web-App-Vulnerability-Discovery-and-Scanning/NDSS-2025__Eagleye-Exposing-Hidden-Web-Interfaces-In-Iot-Devices-Via-Routing-Analysis.pdf`
- **Evocrawl Exploring Web Application Code And State Using Evolutionary Search** (NDSS 2025)  
  [PDF](https://www.ndss-symposium.org/wp-content/uploads/2025-366-paper.pdf) · `papers/Offensive-Papers/Web-App-Vulnerability-Discovery-and-Scanning/NDSS-2025__Evocrawl-Exploring-Web-Application-Code-And-State-Using-Evolutionary-Search.pdf`
- **Yurascanner Leveraging Llms For Task Driven Web App Scanning** (NDSS 2025)  
  [PDF](https://www.ndss-symposium.org/wp-content/uploads/2025-388-paper.pdf) · `papers/Offensive-Papers/Web-App-Vulnerability-Discovery-and-Scanning/NDSS-2025__Yurascanner-Leveraging-Llms-For-Task-Driven-Web-App-Scanning.pdf`
- **Lost in Translation: Exploring the Risks of Web-to-Cross-platform Application Migration** (PoPETs 2025)  
  [PDF](https://petsymposium.org/popets/2025/popets-2025-0117.pdf) · `papers/Offensive-Papers/Web-App-Vulnerability-Discovery-and-Scanning/PoPETs-2025__Lost-in-Translation-Exploring-the-Risks-of-Web-to-Cross-platform-Application-Migration.pdf`
- **Atropos Effective Fuzzing of Web Applications for Server-Side Vulnerabilities** (USENIX-Security 2024)  
  [PDF](https://www.usenix.org/system/files/usenixsecurity24-guler.pdf) · `papers/Offensive-Papers/Web-App-Vulnerability-Discovery-and-Scanning/USENIX-Security-2024__Atropos-Effective-Fuzzing-of-Web-Applications-for-Server-Side-Vulnerabilities.pdf`
- **Web Platform Threats Automated Detection of Web Security Issues With WPT** (USENIX-Security 2024)  
  [PDF](https://www.usenix.org/system/files/usenixsecurity24-bernardo.pdf) · `papers/Offensive-Papers/Web-App-Vulnerability-Discovery-and-Scanning/USENIX-Security-2024__Web-Platform-Threats-Automated-Detection-of-Web-Security-Issues-With-WPT.pdf`
- **Effective Directed Fuzzing with Hierarchical Scheduling for Web Vulnerability Detection** (USENIX-Security 2025)  
  [PDF](https://www.usenix.org/system/files/usenixsecurity25-lin-zihan.pdf) · `papers/Offensive-Papers/Web-App-Vulnerability-Discovery-and-Scanning/USENIX-Security-2025__Effective-Directed-Fuzzing-with-Hierarchical-Scheduling-for-Web-Vulnerability-Detection.pdf`
- **Towards Automatic Detection and Exploitation of Java Web Application Vulnerabilities via Concolic Execution guided by Cross-thread Object Manipulation** (USENIX-Security 2025)  
  [PDF](https://www.usenix.org/system/files/usenixsecurity25-huang-xinyou.pdf) · `papers/Offensive-Papers/Web-App-Vulnerability-Discovery-and-Scanning/USENIX-Security-2025__Towards-Automatic-Detection-and-Exploitation-of-Java-Web-Application-Vulnerabilities-via-Concol.pdf`

### Authentication Identity and Access Attacks (8)
_Attacks on logins, OAuth, credentials, password managers, autofill, FIDO2, QR-login, and identity/age verification._

- **A Security and Usability Analysis of Local Attacks Against FIDO2** (NDSS 2024)  
  [PDF](https://www.ndss-symposium.org/wp-content/uploads/2024-327-paper.pdf) · `papers/Offensive-Papers/Authentication-Identity-and-Access-Attacks/NDSS-2024__A-Security-And-Usability-Analysis-Of-Local-Attacks-Against-Fido2.pdf`
- **The Skeleton Keys A Large Scale Analysis Of Credential Leakage In Mini Apps** (NDSS 2025)  
  [PDF](https://www.ndss-symposium.org/wp-content/uploads/2025-273-paper.pdf) · `papers/Offensive-Papers/Authentication-Identity-and-Access-Attacks/NDSS-2025__The-Skeleton-Keys-A-Large-Scale-Analysis-Of-Credential-Leakage-In-Mini-Apps.pdf`
- **Vault Raider Stealthy Ui Based Attacks Against Password Managers In Desktop Environments** (NDSS 2026)  
  [PDF](https://www.ndss-symposium.org/wp-content/uploads/2026-s1067-paper.pdf) · `papers/Offensive-Papers/Authentication-Identity-and-Access-Attacks/NDSS-2026__Vault-Raider-Stealthy-Ui-Based-Attacks-Against-Password-Managers-In-Desktop-Environments.pdf`
- **Demystifying the (In)Security of QR Code-based Login in Real-world Deployments** (USENIX-Security 2025)  
  [PDF](https://www.usenix.org/system/files/usenixsecurity25-zhang-xin.pdf) · `papers/Offensive-Papers/Authentication-Identity-and-Access-Attacks/USENIX-Security-2025__Demystifying-the-In-Security-of-QR-Code-based-Login-in-Real-world-Deployments.pdf`
- **Phishing Attacks against Password Manager Browser Extensions** (USENIX-Security 2025)  
  [PDF](https://www.usenix.org/system/files/usenixsecurity25-anliker.pdf) · `papers/Offensive-Papers/Authentication-Identity-and-Access-Attacks/USENIX-Security-2025__Phishing-Attacks-against-Password-Manager-Browser-Extensions.pdf`
- **Universal Cross-app Attacks: Exploiting and Securing OAuth 2.0 in Integration Platforms** (USENIX-Security 2025)  
  [PDF](https://www.usenix.org/system/files/usenixsecurity25-luo-kaixuan.pdf) · `papers/Offensive-Papers/Authentication-Identity-and-Access-Attacks/USENIX-Security-2025__Universal-Cross-app-Attacks-Exploiting-and-Securing-OAuth-2-0-in-Integration-Platforms.pdf`
- **AutoFail: Breaking Web Boundaries using Android's Autofill Framework** (USENIX-Security 2026)  
  [PDF](https://www.usenix.org/system/files/usenixsecurity26-lamarca.pdf) · `papers/Offensive-Papers/Authentication-Identity-and-Access-Attacks/USENIX-Security-2026__AutoFail-Breaking-Web-Boundaries-using-Android-s-Autofill-Framework.pdf`
- **X-rated Compliance Theater: An Empirical Evaluation of European Age Verification Systems in Adult Websites** (USENIX-Security 2026)  
  [PDF](https://www.usenix.org/system/files/usenixsecurity26-lavermicocca.pdf) · `papers/Offensive-Papers/Authentication-Identity-and-Access-Attacks/USENIX-Security-2026__X-rated-Compliance-Theater-An-Empirical-Evaluation-of-European-Age-Verification-Systems-in-Adul.pdf`

### Injection Taint and Deserialization (8)
_SQL/command/code injection, taint-style bugs, prototype pollution, and (de)serialization gadget chains._

- **Nodemedic Fine Automatic Detection And Exploit Synthesis For Node Js Vulnerabilities** (NDSS 2025)  
  [PDF](https://www.ndss-symposium.org/wp-content/uploads/2025-1636-paper.pdf) · `papers/Offensive-Papers/Injection-Taint-and-Deserialization/NDSS-2025__Nodemedic-Fine-Automatic-Detection-And-Exploit-Synthesis-For-Node-Js-Vulnerabilities.pdf`
- **Bullseye Detecting Prototype Pollution In Npm Packages With Proof Of Concept Exploits** (NDSS 2026)  
  [PDF](https://www.ndss-symposium.org/wp-content/uploads/2026-s211-paper.pdf) · `papers/Offensive-Papers/Injection-Taint-and-Deserialization/NDSS-2026__Bullseye-Detecting-Prototype-Pollution-In-Npm-Packages-With-Proof-Of-Concept-Exploits.pdf`
- **Firmcross Detecting Taint Style Vulnerabilities In Modern C Lua Hybrid Web Services Of Linux Based Firmware** (NDSS 2026)  
  [PDF](https://www.ndss-symposium.org/wp-content/uploads/2026-s1251-paper.pdf) · `papers/Offensive-Papers/Injection-Taint-and-Deserialization/NDSS-2026__Firmcross-Detecting-Taint-Style-Vulnerabilities-In-Modern-C-Lua-Hybrid-Web-Services-Of-Linux-Ba.pdf`
- **Argus All your PHP Injection-sinks are belong to us** (USENIX-Security 2024)  
  [PDF](https://www.usenix.org/system/files/usenixsecurity24-jahanshahi.pdf) · `papers/Offensive-Papers/Injection-Taint-and-Deserialization/USENIX-Security-2024__Argus-All-your-PHP-Injection-sinks-are-belong-to-us.pdf`
- **GHunter Universal Prototype Pollution Gadgets in JavaScript Runtimes** (USENIX-Security 2024)  
  [PDF](https://www.usenix.org/system/files/usenixsecurity24-cornelissen.pdf) · `papers/Offensive-Papers/Injection-Taint-and-Deserialization/USENIX-Security-2024__GHunter-Universal-Prototype-Pollution-Gadgets-in-JavaScript-Runtimes.pdf`
- **Precise and Effective Gadget Chain Mining through Deserialization Guided Call Graph Construction** (USENIX-Security 2025)  
  [PDF](https://www.usenix.org/system/files/usenixsecurity25-zhang-yiheng.pdf) · `papers/Offensive-Papers/Injection-Taint-and-Deserialization/USENIX-Security-2025__Precise-and-Effective-Gadget-Chain-Mining-through-Deserialization-Guided-Call-Graph-Constructio.pdf`
- **ZIPPER: Static Taint Analysis for PHP Applications with Precision and Efficiency** (USENIX-Security 2025)  
  [PDF](https://www.usenix.org/system/files/usenixsecurity25-wang-xinyi.pdf) · `papers/Offensive-Papers/Injection-Taint-and-Deserialization/USENIX-Security-2025__ZIPPER-Static-Taint-Analysis-for-PHP-Applications-with-Precision-and-Efficiency.pdf`
- **JScamd: An Automated Static Taint Analysis Framework for Detecting Cryptographic API Misuses in JavaScript** (USENIX-Security 2026)  
  [PDF](https://www.usenix.org/system/files/usenixsecurity26-jia-shijie.pdf) · `papers/Offensive-Papers/Injection-Taint-and-Deserialization/USENIX-Security-2026__JScamd-An-Automated-Static-Taint-Analysis-Framework-for-Detecting-Cryptographic-API-Misuses-in.pdf`

### Phishing Scams and Web Abuse (5)
_Phishing, scam campaigns, URL-shortener/e-commerce abuse, and evasion of phishing detectors._

- **Like Comment Get Scammed Characterizing Comment Scams on Media Platforms** (NDSS 2024)  
  [PDF](https://www.ndss-symposium.org/wp-content/uploads/2024-60-paper.pdf) · `papers/Offensive-Papers/Phishing-Scams-and-Web-Abuse/NDSS-2024__Like-Comment-Get-Scammed-Characterizing-Comment-Scams-On-Media-Platforms.pdf`
- **The Dark Side of E-Commerce Dropshipping Abuse as a Business Model** (NDSS 2024)  
  [PDF](https://www.ndss-symposium.org/wp-content/uploads/2024-39-paper.pdf) · `papers/Offensive-Papers/Phishing-Scams-and-Web-Abuse/NDSS-2024__The-Dark-Side-Of-E-Commerce-Dropshipping-Abuse-As-A-Business-Model.pdf`
- **Misdirection Of Trust Demystifying The Abuse Of Dedicated Url Shortening Service** (NDSS 2025)  
  [PDF](https://www.ndss-symposium.org/wp-content/uploads/2025-927-paper.pdf) · `papers/Offensive-Papers/Phishing-Scams-and-Web-Abuse/NDSS-2025__Misdirection-Of-Trust-Demystifying-The-Abuse-Of-Dedicated-Url-Shortening-Service.pdf`
- **It Doesn't Look Like Anything to Me Using Diffusion Model to Subvert Visual Phishing Detectors** (USENIX-Security 2024)  
  [PDF](https://www.usenix.org/system/files/usenixsecurity24-hao-qingying.pdf) · `papers/Offensive-Papers/Phishing-Scams-and-Web-Abuse/USENIX-Security-2024__It-Doesn-t-Look-Like-Anything-to-Me-Using-Diffusion-Model-to-Subvert-Visual-Phishing-Detec.pdf`
- **A Large-Scale Study of Personalized Phishing using Large Language Models** (USENIX-Security 2026)  
  [PDF](https://www.usenix.org/system/files/usenixsecurity26-czybik.pdf) · `papers/Offensive-Papers/Phishing-Scams-and-Web-Abuse/USENIX-Security-2026__A-Large-Scale-Study-of-Personalized-Phishing-using-Large-Language-Models.pdf`

### Runtime Engine and Browser Internals (5)
_Bugs and exploitation in JS engines, the PHP interpreter, and browser policy-enforcement internals._

- **Dumpling Fine Grained Differential Javascript Engine Fuzzing** (NDSS 2025)  
  [PDF](https://www.ndss-symposium.org/wp-content/uploads/2025-1411-paper.pdf) · `papers/Offensive-Papers/Runtime-Engine-and-Browser-Internals/NDSS-2025__Dumpling-Fine-Grained-Differential-Javascript-Engine-Fuzzing.pdf`
- **OptFuzz Optimization Path Guided Fuzzing for JavaScript JIT Compilers** (USENIX-Security 2024)  
  [PDF](https://www.usenix.org/system/files/usenixsecurity24-wang-jiming.pdf) · `papers/Offensive-Papers/Runtime-Engine-and-Browser-Internals/USENIX-Security-2024__OptFuzz-Optimization-Path-Guided-Fuzzing-for-JavaScript-JIT-Compilers.pdf`
- **Fuzzing the PHP Interpreter via Dataflow Fusion** (USENIX-Security 2025)  
  [PDF](https://www.usenix.org/system/files/usenixsecurity25-jiang-yuancheng.pdf) · `papers/Offensive-Papers/Runtime-Engine-and-Browser-Internals/USENIX-Security-2025__Fuzzing-the-PHP-Interpreter-via-Dataflow-Fusion.pdf`
- **BUIzz: Finding Policy Enforcement Bugs via Interaction Simulation on the Browser User Interface** (USENIX-Security 2026)  
  [PDF](https://www.usenix.org/system/files/usenixsecurity26-jung.pdf) · `papers/Offensive-Papers/Runtime-Engine-and-Browser-Internals/USENIX-Security-2026__BUIzz-Finding-Policy-Enforcement-Bugs-via-Interaction-Simulation-on-the-Browser-User-Interface.pdf`
- **Melting the Flesh of PHP's Memory Hardening** (USENIX-Security 2026)  
  [PDF](https://www.usenix.org/system/files/usenixsecurity26-wu-yifan.pdf) · `papers/Offensive-Papers/Runtime-Engine-and-Browser-Internals/USENIX-Security-2026__Melting-the-Flesh-of-PHP-s-Memory-Hardening.pdf`

### XSS and DOM (4)
_Cross-site scripting, DOM-based XSS, and DOM clobbering._

- **Dom Xss Detection Via Webpage Interaction Fuzzing And Url Component Synthesis** (NDSS 2026)  
  [PDF](https://www.ndss-symposium.org/wp-content/uploads/2026-s1467-paper.pdf) · `papers/Offensive-Papers/XSS-and-DOM/NDSS-2026__Dom-Xss-Detection-Via-Webpage-Interaction-Fuzzing-And-Url-Component-Synthesis.pdf`
- **Spider-Scents Grey-box Database-aware Web Scanning for Stored XSS** (USENIX-Security 2024)  
  [PDF](https://www.usenix.org/system/files/usenixsecurity24-olsson.pdf) · `papers/Offensive-Papers/XSS-and-DOM/USENIX-Security-2024__Spider-Scents-Grey-box-Database-aware-Web-Scanning-for-Stored-XSS.pdf`
- **The DOMino Effect: Detecting and Exploiting DOM Clobbering Gadgets via Concolic Execution with Symbolic DOM** (USENIX-Security 2025)  
  [PDF](https://www.usenix.org/system/files/usenixsecurity25-liu-zhengyu.pdf) · `papers/Offensive-Papers/XSS-and-DOM/USENIX-Security-2025__The-DOMino-Effect-Detecting-and-Exploiting-DOM-Clobbering-Gadgets-via-Concolic-Execution-with-S.pdf`
- **XSSky: Detecting XSS Vulnerabilities through Local Path-Persistent Fuzzing** (USENIX-Security 2025)  
  [PDF](https://www.usenix.org/system/files/usenixsecurity25-shi-youkun.pdf) · `papers/Offensive-Papers/XSS-and-DOM/USENIX-Security-2025__XSSky-Detecting-XSS-Vulnerabilities-through-Local-Path-Persistent-Fuzzing.pdf`

### DoS and Availability (2)
_Denial-of-service and amplification against web containers and CDNs._

- **CDN Cannon Exploiting CDN Back-to-Origin Strategies for Amplification Attacks** (USENIX-Security 2024)  
  [PDF](https://www.usenix.org/system/files/usenixsecurity24-lin-ziyu.pdf) · `papers/Offensive-Papers/DoS-and-Availability/USENIX-Security-2024__CDN-Cannon-Exploiting-CDN-Back-to-Origin-Strategies-for-Amplification-Attacks.pdf`
- **Careless Retention and Management: Understanding and Detecting Data Retention Denial-of-Service Vulnerabilities in Java Web Containers** (USENIX-Security 2025)  
  [PDF](https://www.usenix.org/system/files/usenixsecurity25-lian.pdf) · `papers/Offensive-Papers/DoS-and-Availability/USENIX-Security-2025__Careless-Retention-and-Management-Understanding-and-Detecting-Data-Retention-Denial-of-Service.pdf`

### Domain and DNS Takeover (2)
_Domain/subdomain and DNS-based hijacking that enables web takeover._

- **Cross the Zone Toward a Covert Domain Hijacking via Shared DNS Infrastructure** (USENIX-Security 2024)  
  [PDF](https://www.usenix.org/system/files/usenixsecurity24-zhang-yunyi-zone.pdf) · `papers/Offensive-Papers/Domain-and-DNS-Takeover/USENIX-Security-2024__Cross-the-Zone-Toward-a-Covert-Domain-Hijacking-via-Shared-DNS-Infrastructure.pdf`
- **Alias Equals Zone? Large-Scale and Stealthy Takeover of Domain Hosting Service via CNAME-Following Cross-Domain Verification** (USENIX-Security 2026)  
  [PDF](https://www.usenix.org/system/files/usenixsecurity26-li-ruixuan.pdf) · `papers/Offensive-Papers/Domain-and-DNS-Takeover/USENIX-Security-2026__Alias-Equals-Zone-Large-Scale-and-Stealthy-Takeover-of-Domain-Hosting-Service-via-CNAME-Followi.pdf`

### Payment and Authorization Attacks (2)
_Breaking third-party online payments and emerging web-payment protocols._

- **When Authorization Loses Its Meaning: Breaking and Fixing Third-Party Online Payments** (USENIX-Security 2026)  
  [PDF](https://www.usenix.org/system/files/usenixsecurity26-xiao.pdf) · `papers/Offensive-Papers/Payment-and-Authorization-Attacks/USENIX-Security-2026__When-Authorization-Loses-Its-Meaning-Breaking-and-Fixing-Third-Party-Online-Payments.pdf`
- **When HTTP 402 Meets the Blockchain: Risks on Emerging x402 Payments** (USENIX-Security 2026)  
  [PDF](https://www.usenix.org/system/files/usenixsecurity26-wang-qinying.pdf) · `papers/Offensive-Papers/Payment-and-Authorization-Attacks/USENIX-Security-2026__When-HTTP-402-Meets-the-Blockchain-Risks-on-Emerging-x402-Payments.pdf`

### Web Agent and LLM Attacks (2)
_Red-teaming and threat analysis of LLM-driven web agents and web-enabled LLMs._

- **When LLMs Go Online The Emerging Threat of Web-Enabled LLMs** (USENIX-Security 2025)  
  [PDF](https://www.usenix.org/system/files/usenixsecurity25-kim-hanna.pdf) · `papers/Offensive-Papers/Web-Agent-and-LLM-Attacks/USENIX-Security-2025__When-LLMs-Go-Online-The-Emerging-Threat-of-Web-Enabled-LLMs.pdf`
- **MUZZLE: Adaptive Agentic Red-Teaming of Web Agents Against Indirect Prompt Injection Attacks** (USENIX-Security 2026)  
  [PDF](https://www.usenix.org/system/files/usenixsecurity26-syros.pdf) · `papers/Offensive-Papers/Web-Agent-and-LLM-Attacks/USENIX-Security-2026__MUZZLE-Adaptive-Agentic-Red-Teaming-of-Web-Agents-Against-Indirect-Prompt-Injection-Attacks.pdf`

---

## Defensive-Papers (61)

Detection, mitigation, hardening, privacy/compliance enforcement, and systematizations that strengthen the web.

### Anti Tracking and Privacy Defenses (13)
_Tracker/fingerprint detection and blocking, and privacy-preserving advertising mechanisms._

- **FP-Fed Privacy-Preserving Federated Detection of Browser Fingerprinting** (NDSS 2024)  
  [PDF](https://www.ndss-symposium.org/wp-content/uploads/2024-360-paper.pdf) · `papers/Defensive-Papers/Anti-Tracking-and-Privacy-Defenses/NDSS-2024__Fp-Fed-Privacy-Preserving-Federated-Detection-Of-Browser-Fingerprinting.pdf`
- **Duumviri Detecting Trackers And Mixed Trackers With A Breakage Detector** (NDSS 2025)  
  [PDF](https://www.ndss-symposium.org/wp-content/uploads/2025-267-paper.pdf) · `papers/Defensive-Papers/Anti-Tracking-and-Privacy-Defenses/NDSS-2025__Duumviri-Detecting-Trackers-And-Mixed-Trackers-With-A-Breakage-Detector.pdf`
- **Block Cookies Not Websites Analysing Mental Models and Usability of the Privacy-Preserving Browser Extension CookieBlock** (PoPETs 2024)  
  [PDF](https://petsymposium.org/popets/2024/popets-2024-0012.pdf) · `papers/Defensive-Papers/Anti-Tracking-and-Privacy-Defenses/PoPETs-2024__Block-Cookies-Not-Websites-Analysing-Mental-Models-and-Usability-of-the-Privacy-Preserving.pdf`
- **Evaluating Google's Protected Audience Protocol** (PoPETs 2024)  
  [PDF](https://petsymposium.org/popets/2024/popets-2024-0147.pdf) · `papers/Defensive-Papers/Anti-Tracking-and-Privacy-Defenses/PoPETs-2024__Evaluating-Google-s-Protected-Audience-Protocol.pdf`
- **FP-tracer Fine-grained Browser Fingerprinting Detection via Taint-tracking and Entropy-based Thresholds** (PoPETs 2024)  
  [PDF](https://petsymposium.org/popets/2024/popets-2024-0092.pdf) · `papers/Defensive-Papers/Anti-Tracking-and-Privacy-Defenses/PoPETs-2024__FP-tracer-Fine-grained-Browser-Fingerprinting-Detection-via-Taint-tracking-and-Entropy-bas.pdf`
- **Summary Reports Optimization in the Privacy Sandbox Attribution Reporting API** (PoPETs 2024)  
  [PDF](https://petsymposium.org/popets/2024/popets-2024-0132.pdf) · `papers/Defensive-Papers/Anti-Tracking-and-Privacy-Defenses/PoPETs-2024__Summary-Reports-Optimization-in-the-Privacy-Sandbox-Attribution-Reporting-API.pdf`
- **The Devil is in the Details Detection Measurement and Lawfulness of Server-Side Tracking on the Web** (PoPETs 2024)  
  [PDF](https://petsymposium.org/popets/2024/popets-2024-0125.pdf) · `papers/Defensive-Papers/Anti-Tracking-and-Privacy-Defenses/PoPETs-2024__The-Devil-is-in-the-Details-Detection-Measurement-and-Lawfulness-of-Server-Side-Tracking-o.pdf`
- **Website Data Transparency in the Browser** (PoPETs 2024)  
  [PDF](https://petsymposium.org/popets/2024/popets-2024-0048.pdf) · `papers/Defensive-Papers/Anti-Tracking-and-Privacy-Defenses/PoPETs-2024__Website-Data-Transparency-in-the-Browser.pdf`
- **Beyond the Request: Harnessing HTTP Response Headers for Cross-Browser Web Tracker Detection** (PoPETs 2025)  
  [PDF](https://petsymposium.org/popets/2025/popets-2025-0007.pdf) · `papers/Defensive-Papers/Anti-Tracking-and-Privacy-Defenses/PoPETs-2025__Beyond-the-Request-Harnessing-HTTP-Response-Headers-for-Cross-Browser-Web-Tracker-Detection.pdf`
- **An Improved Entropy Measure for Web Browser Fingerprinting Risk** (PoPETs 2026)  
  [PDF](https://petsymposium.org/popets/2026/popets-2026-0102.pdf) · `papers/Defensive-Papers/Anti-Tracking-and-Privacy-Defenses/PoPETs-2026__An-Improved-Entropy-Measure-for-Web-Browser-Fingerprinting-Risk.pdf`
- **From Syntactic Matching to Taint Tracking and Back: A Comparative Study of Web Tracking Detection** (PoPETs 2026)  
  [PDF](https://petsymposium.org/popets/2026/popets-2026-0122.pdf) · `papers/Defensive-Papers/Anti-Tracking-and-Privacy-Defenses/PoPETs-2026__From-Syntactic-Matching-to-Taint-Tracking-and-Back-A-Comparative-Study-of-Web-Tracking-Detectio.pdf`
- **Arcanum Detecting and Evaluating the Privacy Risks of Browser Extensions on Web Pages and Web Content** (USENIX-Security 2024)  
  [PDF](https://www.usenix.org/system/files/usenixsecurity24-xie-qinge.pdf) · `papers/Defensive-Papers/Anti-Tracking-and-Privacy-Defenses/USENIX-Security-2024__Arcanum-Detecting-and-Evaluating-the-Privacy-Risks-of-Browser-Extensions-on-Web-Pages-and.pdf`
- **PURL Safe and Effective Sanitization of Link Decoration** (USENIX-Security 2024)  
  [PDF](https://www.usenix.org/system/files/usenixsecurity24-munir.pdf) · `papers/Defensive-Papers/Anti-Tracking-and-Privacy-Defenses/USENIX-Security-2024__PURL-Safe-and-Effective-Sanitization-of-Link-Decoration.pdf`

### Phishing and Scam Detection (10)
_Detecting phishing and scam websites, including ML/LLM and reference-based detectors._

- **Scammagnifier Piercing The Veil Of Fraudulent Shopping Website Campaigns** (NDSS 2025)  
  [PDF](https://www.ndss-symposium.org/wp-content/uploads/2025-763-paper.pdf) · `papers/Defensive-Papers/Phishing-and-Scam-Detection/NDSS-2025__Scammagnifier-Piercing-The-Veil-Of-Fraudulent-Shopping-Website-Campaigns.pdf`
- **Ctphishcapture Uncovering Credential Theft Based Phishing Scams Targeting Cryptocurrency Wallets** (NDSS 2026)  
  [PDF](https://www.ndss-symposium.org/wp-content/uploads/2026-f2854-paper.pdf) · `papers/Defensive-Papers/Phishing-and-Scam-Detection/NDSS-2026__Ctphishcapture-Uncovering-Credential-Theft-Based-Phishing-Scams-Targeting-Cryptocurrency-Wallet.pdf`
- **LOKI Proactively Discovering Online Scam Websites by Mining Toxic Search Queries** (NDSS 2026)  
  [PDF](https://www.ndss-symposium.org/wp-content/uploads/2026-s184-paper.pdf) · `papers/Defensive-Papers/Phishing-and-Scam-Detection/NDSS-2026__Loki-Proactively-Discovering-Online-Scam-Websites-By-Mining-Toxic-Search-Queries.pdf`
- **PhishLang A Real-Time Fully Client-Side Phishing Detection Framework Using MobileBERT** (NDSS 2026)  
  [PDF](https://www.ndss-symposium.org/wp-content/uploads/2026-s1037-paper.pdf) · `papers/Defensive-Papers/Phishing-and-Scam-Detection/NDSS-2026__Phishlang-A-Real-Time-Fully-Client-Side-Phishing-Detection-Framework-Using-Mobilebert.pdf`
- **KnowPhish: Large Language Models Meet Multimodal Knowledge Graphs for Enhancing Reference-Based Phishing Detection** (USENIX-Security 2024)  
  [PDF](https://www.usenix.org/system/files/usenixsecurity24-li-yuexin.pdf) · `papers/Defensive-Papers/Phishing-and-Scam-Detection/USENIX-Security-2024__KnowPhish-Large-Language-Models-Meet-Multimodal-Knowledge-Graphs-for-Enhancing-Reference-B.pdf`
- **Less Defined Knowledge and More True Alarms: Reference-based Phishing Detection without a Pre-defined Reference List** (USENIX-Security 2024)  
  [PDF](https://www.usenix.org/system/files/usenixsecurity24-liu-ruofan.pdf) · `papers/Defensive-Papers/Phishing-and-Scam-Detection/USENIX-Security-2024__Less-Defined-Knowledge-and-More-True-Alarms-Reference-based-Phishing-Detection-without-a-P.pdf`
- **PhishDecloaker: Detecting CAPTCHA-cloaked Phishing Websites via Hybrid Vision-based Interactive Models** (USENIX-Security 2024)  
  [PDF](https://www.usenix.org/system/files/usenixsecurity24-teoh.pdf) · `papers/Defensive-Papers/Phishing-and-Scam-Detection/USENIX-Security-2024__PhishDecloaker-Detecting-CAPTCHA-cloaked-Phishing-Websites-via-Hybrid-Vision-based-Interac.pdf`
- **Evaluating the Effectiveness and Robustness of Visual Similarity-based Phishing Detection Models** (USENIX-Security 2025)  
  [PDF](https://www.usenix.org/system/files/usenixsecurity25-ji.pdf) · `papers/Defensive-Papers/Phishing-and-Scam-Detection/USENIX-Security-2025__Evaluating-the-Effectiveness-and-Robustness-of-Visual-Similarity-based-Phishing-Detection.pdf`
- **Designing Wallet-Based User Intervention for Approval Phishing Mitigation** (USENIX-Security 2026)  
  [PDF](https://www.usenix.org/system/files/usenixsecurity26-guan.pdf) · `papers/Defensive-Papers/Phishing-and-Scam-Detection/USENIX-Security-2026__Designing-Wallet-Based-User-Intervention-for-Approval-Phishing-Mitigation.pdf`
- **SoK: PHILTER: Uncovering Security and Functional Gaps in AI-based Phishing Website Detection Literature via an LLM-based Reasoning Framework** (USENIX-Security 2026)  
  [PDF](https://www.usenix.org/system/files/usenixsecurity26-alam.pdf) · `papers/Defensive-Papers/Phishing-and-Scam-Detection/USENIX-Security-2026__SoK-PHILTER-Uncovering-Security-and-Functional-Gaps-in-AI-based-Phishing-Website-Detection-Lite.pdf`

### Privacy Compliance and Consent (10)
_GDPR/CCPA compliance, cookie-consent and opt-out/GPC measurement and enforcement._

- **A Large-Scale Study of Cookie Banner Interaction Tools and their Impact on Users Privacy** (PoPETs 2024)  
  [PDF](https://petsymposium.org/popets/2024/popets-2024-0002.pdf) · `papers/Defensive-Papers/Privacy-Compliance-and-Consent/PoPETs-2024__A-Large-Scale-Study-of-Cookie-Banner-Interaction-Tools-and-their-Impact-on-Users-Privacy.pdf`
- **Generalizable Active Privacy Choice Designing a Graphical User Interface for Global Privacy Control** (PoPETs 2024)  
  [PDF](https://petsymposium.org/popets/2024/popets-2024-0015.pdf) · `papers/Defensive-Papers/Privacy-Compliance-and-Consent/PoPETs-2024__Generalizable-Active-Privacy-Choice-Designing-a-Graphical-User-Interface-for-Global-Privac.pdf`
- **Johnny Still Can't Opt-out Assessing the IAB CCPA Compliance Framework** (PoPETs 2024)  
  [PDF](https://petsymposium.org/popets/2024/popets-2024-0120.pdf) · `papers/Defensive-Papers/Privacy-Compliance-and-Consent/PoPETs-2024__Johnny-Still-Can-t-Opt-out-Assessing-the-IAB-CCPA-Compliance-Framework.pdf`
- **Opted Out Yet Tracked Are Regulations Enough to Protect Your Privacy** (PoPETs 2024)  
  [PDF](https://petsymposium.org/popets/2024/popets-2024-0016.pdf) · `papers/Defensive-Papers/Privacy-Compliance-and-Consent/PoPETs-2024__Opted-Out-Yet-Tracked-Are-Regulations-Enough-to-Protect-Your-Privacy.pdf`
- **Johnny Can't Revoke Consent Either: Measuring Compliance of Consent Revocation on the Web** (PoPETs 2025)  
  [PDF](https://petsymposium.org/popets/2025/popets-2025-0133.pdf) · `papers/Defensive-Papers/Privacy-Compliance-and-Consent/PoPETs-2025__Johnny-Can-t-Revoke-Consent-Either-Measuring-Compliance-of-Consent-Revocation-on-the-Web.pdf`
- **Making Web Applications GDPR Compliant: A Comparative Evaluation of GDPR-Enforcement Frameworks** (PoPETs 2025)  
  [PDF](https://petsymposium.org/popets/2025/popets-2025-0157.pdf) · `papers/Defensive-Papers/Privacy-Compliance-and-Consent/PoPETs-2025__Making-Web-Applications-GDPR-Compliant-A-Comparative-Evaluation-of-GDPR-Enforcement-Frameworks.pdf`
- **Automated Large-Scale Analysis of Cookie Notice Compliance** (USENIX-Security 2024)  
  [PDF](https://www.usenix.org/system/files/usenixsecurity24-bouhoula.pdf) · `papers/Defensive-Papers/Privacy-Compliance-and-Consent/USENIX-Security-2024__Automated-Large-Scale-Analysis-of-Cookie-Notice-Compliance.pdf`
- **The Effect of Design Patterns on Present and Future Cookie Consent Decisions** (USENIX-Security 2024)  
  [PDF](https://www.usenix.org/system/files/usenixsecurity24-bielova.pdf) · `papers/Defensive-Papers/Privacy-Compliance-and-Consent/USENIX-Security-2024__The-Effect-of-Design-Patterns-on-Present-and-Future-Cookie-Consent-Decisions.pdf`
- **Navigating Cookie Consent Violations Across the Globe** (USENIX-Security 2025)  
  [PDF](https://www.usenix.org/system/files/usenixsecurity25-tang.pdf) · `papers/Defensive-Papers/Privacy-Compliance-and-Consent/USENIX-Security-2025__Navigating-Cookie-Consent-Violations-Across-the-Globe.pdf`
- **Websites' Global Privacy Control Compliance at Scale and over Time** (USENIX-Security 2025)  
  [PDF](https://www.usenix.org/system/files/usenixsecurity25-hausladen.pdf) · `papers/Defensive-Papers/Privacy-Compliance-and-Consent/USENIX-Security-2025__Websites-Global-Privacy-Control-Compliance-at-Scale-and-over-Time.pdf`

### Authentication and Passkey Defenses (8)
_Passkeys/WebAuthn, account recovery, OAuth minimization, and SSO defenses._

- **Post-quantum XML and SAML Single Sign-On** (PoPETs 2024)  
  [PDF](https://petsymposium.org/popets/2024/popets-2024-0128.pdf) · `papers/Defensive-Papers/Authentication-and-Passkey-Defenses/PoPETs-2024__Post-quantum-XML-and-SAML-Single-Sign-On.pdf`
- **SoK: Web Authentication and Recovery in the Age of End-to-End Encryption** (PoPETs 2025)  
  [PDF](https://petsymposium.org/popets/2025/popets-2025-0113.pdf) · `papers/Defensive-Papers/Authentication-and-Passkey-Defenses/PoPETs-2025__SoK-Web-Authentication-and-Recovery-in-the-Age-of-End-to-End-Encryption.pdf`
- **OAuthHub: Mitigating OAuth Data Overaccess through a Local Data Hub** (PoPETs 2026)  
  [PDF](https://petsymposium.org/popets/2026/popets-2026-0098.pdf) · `papers/Defensive-Papers/Authentication-and-Passkey-Defenses/PoPETs-2026__OAuthHub-Mitigating-OAuth-Data-Overaccess-through-a-Local-Data-Hub.pdf`
- **Secure Account Recovery for a Privacy-Preserving Web Service** (USENIX-Security 2024)  
  [PDF](https://www.usenix.org/system/files/usenixsecurity24-little.pdf) · `papers/Defensive-Papers/Authentication-and-Passkey-Defenses/USENIX-Security-2024__Secure-Account-Recovery-for-a-Privacy-Preserving-Web-Service.pdf`
- **Why Aren't We Using Passkeys Obstacles Companies Face Deploying FIDO2 Passwordless Authentication** (USENIX-Security 2024)  
  [PDF](https://www.usenix.org/system/files/usenixsecurity24-lassak.pdf) · `papers/Defensive-Papers/Authentication-and-Passkey-Defenses/USENIX-Security-2024__Why-Aren-t-We-Using-Passkeys-Obstacles-Companies-Face-Deploying-FIDO2-Passwordless-Authent.pdf`
- **Detecting Compromise of Passkey Storage on the Cloud** (USENIX-Security 2025)  
  [PDF](https://www.usenix.org/system/files/usenixsecurity25-islam.pdf) · `papers/Defensive-Papers/Authentication-and-Passkey-Defenses/USENIX-Security-2025__Detecting-Compromise-of-Passkey-Storage-on-the-Cloud.pdf`
- **Maybe there's only one passkey Challenges Investigating and Remediating Adversarial Passkeys** (USENIX-Security 2026)  
  [PDF](https://www.usenix.org/system/files/usenixsecurity26-daffalla.pdf) · `papers/Defensive-Papers/Authentication-and-Passkey-Defenses/USENIX-Security-2026__Maybe-there-s-only-one-passkey-Challenges-Investigating-and-Remediating-Adversarial-Passke.pdf`
- **The State of Passkeys: Studying the Adoption and Security of Passkeys on the Web** (USENIX-Security 2026)  
  [PDF](https://www.usenix.org/system/files/usenixsecurity26-jannett.pdf) · `papers/Defensive-Papers/Authentication-and-Passkey-Defenses/USENIX-Security-2026__The-State-of-Passkeys-Studying-the-Adoption-and-Security-of-Passkeys-on-the-Web.pdf`

### PKI and Transport Security (4)
_Web PKI, certificate transparency, domain validation, and HSTS._

- **Certificate Transparency Revisited The Public Inspections on Third-party Monitors** (NDSS 2024)  
  [PDF](https://www.ndss-symposium.org/wp-content/uploads/2024-834-paper.pdf) · `papers/Defensive-Papers/PKI-and-Transport-Security/NDSS-2024__Certificate-Transparency-Revisited-The-Public-Inspections-On-Third-Party-Monitors.pdf`
- **Ctng Secure Certificate And Revocation Transparency** (NDSS 2026)  
  [PDF](https://www.ndss-symposium.org/wp-content/uploads/2026-s213-paper.pdf) · `papers/Defensive-Papers/PKI-and-Transport-Security/NDSS-2026__Ctng-Secure-Certificate-And-Revocation-Transparency.pdf`
- **CoStricTor Collaborative HTTP Strict Transport Security in Tor Browser** (PoPETs 2024)  
  [PDF](https://petsymposium.org/popets/2024/popets-2024-0020.pdf) · `papers/Defensive-Papers/PKI-and-Transport-Security/PoPETs-2024__CoStricTor-Collaborative-HTTP-Strict-Transport-Security-in-Tor-Browser.pdf`
- **Cryptographically-Secured Domain Validation** (PoPETs 2026)  
  [PDF](https://petsymposium.org/popets/2026/popets-2026-0056.pdf) · `papers/Defensive-Papers/PKI-and-Transport-Security/PoPETs-2026__Cryptographically-Secured-Domain-Validation.pdf`

### Vulnerability Mitigation and Hardening (4)
_Runtime containment, SSRF/deserialization defenses, and hardening of web applications._

- **Automatic Policy Synthesis and Enforcement for Protecting Untrusted Deserialization** (NDSS 2024)  
  [PDF](https://www.ndss-symposium.org/wp-content/uploads/2024-53-paper.pdf) · `papers/Defensive-Papers/Vulnerability-Mitigation-and-Hardening/NDSS-2024__Automatic-Policy-Synthesis-And-Enforcement-For-Protecting-Untrusted-Deserialization.pdf`
- **QUACK Hindering Deserialization Attacks via Static Duck Typing** (NDSS 2024)  
  [PDF](https://www.ndss-symposium.org/wp-content/uploads/2024-1015-paper.pdf) · `papers/Defensive-Papers/Vulnerability-Mitigation-and-Hardening/NDSS-2024__Quack-Hindering-Deserialization-Attacks-Via-Static-Duck-Typing.pdf`
- **SSRF vs Developers A Study of SSRF-Defenses in PHP Applications** (USENIX-Security 2024)  
  [PDF](https://www.usenix.org/system/files/usenixsecurity24-wessels.pdf) · `papers/Defensive-Papers/Vulnerability-Mitigation-and-Hardening/USENIX-Security-2024__SSRF-vs-Developers-A-Study-of-SSRF-Defenses-in-PHP-Applications.pdf`
- **Kintsugi: Empowering LLMs to Mitigate Web Vulnerabilities via Runtime Policy Injection** (USENIX-Security 2026)  
  [PDF](https://www.usenix.org/system/files/usenixsecurity26-peng-yihao.pdf) · `papers/Defensive-Papers/Vulnerability-Mitigation-and-Hardening/USENIX-Security-2026__Kintsugi-Empowering-LLMs-to-Mitigate-Web-Vulnerabilities-via-Runtime-Policy-Injection.pdf`

### Web Attack and Malware Detection (4)
_Runtime detection of web attacks and analysis/deobfuscation of malicious JavaScript, plus web forensics._

- **Achieving Interpretable Dl Based Web Attack Detection Through Malicious Payload Localization** (NDSS 2026)  
  [PDF](https://www.ndss-symposium.org/wp-content/uploads/2026-s1029-paper.pdf) · `papers/Defensive-Papers/Web-Attack-and-Malware-Detection/NDSS-2026__Achieving-Interpretable-Dl-Based-Web-Attack-Detection-Through-Malicious-Payload-Localization.pdf`
- **From Obfuscated To Obvious A Comprehensive Javascript Deobfuscation Tool For Security Analysis** (NDSS 2026)  
  [PDF](https://www.ndss-symposium.org/wp-content/uploads/2026-f2198-paper.pdf) · `papers/Defensive-Papers/Web-Attack-and-Malware-Detection/NDSS-2026__From-Obfuscated-To-Obvious-A-Comprehensive-Javascript-Deobfuscation-Tool-For-Security-Analysis.pdf`
- **FV8 A Forced Execution JavaScript Engine for Detecting Evasive Techniques** (USENIX-Security 2024)  
  [PDF](https://www.usenix.org/system/files/usenixsecurity24-pantelaios.pdf) · `papers/Defensive-Papers/Web-Attack-and-Malware-Detection/USENIX-Security-2024__FV8-A-Forced-Execution-JavaScript-Engine-for-Detecting-Evasive-Techniques.pdf`
- **WEBRR A Forensic System for Replaying and Investigating Web-Based Attacks in The Modern Web** (USENIX-Security 2024)  
  [PDF](https://www.usenix.org/system/files/usenixsecurity24-allen.pdf) · `papers/Defensive-Papers/Web-Attack-and-Malware-Detection/USENIX-Security-2024__WEBRR-A-Forensic-System-for-Replaying-and-Investigating-Web-Based-Attacks-in-The-Modern-We.pdf`

### Web Agent and LLM Security (3)
_Defenses/benchmarks for web agents, prompt-injection resistance, and safe AI web search._

- **WebSP-Eval: Evaluating Web Agents on Website Security and Privacy Tasks** (PoPETs 2026)  
  [PDF](https://petsymposium.org/popets/2026/popets-2026-0140.pdf) · `papers/Defensive-Papers/Web-Agent-and-LLM-Security/PoPETs-2026__WebSP-Eval-Evaluating-Web-Agents-on-Website-Security-and-Privacy-Tasks.pdf`
- **StruQ Defending Against Prompt Injection with Structured Queries** (USENIX-Security 2025)  
  [PDF](https://www.usenix.org/system/files/usenixsecurity25-chen-sizhe.pdf) · `papers/Defensive-Papers/Web-Agent-and-LLM-Security/USENIX-Security-2025__StruQ-Defending-Against-Prompt-Injection-with-Structured-Queries.pdf`
- **Unsafe LLM-Based Search Quantitative Analysis and Mitigation of Safety Risks in AI Web Search** (USENIX-Security 2025)  
  [PDF](https://www.usenix.org/system/files/usenixsecurity25-luo-zeren.pdf) · `papers/Defensive-Papers/Web-Agent-and-LLM-Security/USENIX-Security-2025__Unsafe-LLM-Based-Search-Quantitative-Analysis-and-Mitigation-of-Safety-Risks-in-AI-Web-Sea.pdf`

### Measurement Tools and SoK (2)
_Reusable web-measurement infrastructure and systematization-of-knowledge on web methods._

- **SoK State of the Krawlers Evaluating the Effectiveness of Crawling Algorithms for Web Security Measurements** (USENIX-Security 2024)  
  [PDF](https://www.usenix.org/system/files/usenixsecurity24-stafeev.pdf) · `papers/Defensive-Papers/Measurement-Tools-and-SoK/USENIX-Security-2024__SoK-State-of-the-Krawlers-Evaluating-the-Effectiveness-of-Crawling-Algorithms-for-Web-Secu.pdf`
- **Web Execution Bundles: Reproducible, Accurate, and Archivable Web Measurements** (USENIX-Security 2025)  
  [PDF](https://www.usenix.org/system/files/usenixsecurity25-hantke.pdf) · `papers/Defensive-Papers/Measurement-Tools-and-SoK/USENIX-Security-2025__Web-Execution-Bundles-Reproducible-Accurate-and-Archivable-Web-Measurements.pdf`

### Supply Chain Security (2)
_npm and multi-registry package supply-chain security._

- **From Noise To Signal Precisely Identify Affected Packages Of Known Vulnerabilities In Npm Ecosystem** (NDSS 2026)  
  [PDF](https://www.ndss-symposium.org/wp-content/uploads/2026-f1902-paper.pdf) · `papers/Defensive-Papers/Supply-Chain-Security/NDSS-2026__From-Noise-To-Signal-Precisely-Identify-Affected-Packages-Of-Known-Vulnerabilities-In-Npm-Ecosy.pdf`
- **DONAPI Malicious NPM Packages Detector using Behavior Sequence Knowledge Mapping** (USENIX-Security 2024)  
  [PDF](https://www.usenix.org/system/files/usenixsecurity24-huang-cheng.pdf) · `papers/Defensive-Papers/Supply-Chain-Security/USENIX-Security-2024__DONAPI-Malicious-NPM-Packages-Detector-using-Behavior-Sequence-Knowledge-Mapping.pdf`

### Content Protection and Anti Crawling (1)
_Protecting web content from unauthorized crawling and LLM scraping._

- **Expshield Safeguarding Web Text From Unauthorized Crawling And Llm Exploitation** (NDSS 2026)  
  [PDF](https://www.ndss-symposium.org/wp-content/uploads/2026-f11-paper.pdf) · `papers/Defensive-Papers/Content-Protection-and-Anti-Crawling/NDSS-2026__Expshield-Safeguarding-Web-Text-From-Unauthorized-Crawling-And-Llm-Exploitation.pdf`

---

## Notes on scope

**Venues.** NDSS, USENIX Security, and PoPETs publish open-access PDFs. S&P/Oakland, CCS, RAID, DIMVA, and ACSAC
publish via IEEE/ACM/Springer paywalls; Black Hat / DEF CON release slides and whitepapers rather than peer-reviewed papers,
so they are out of scope for an automatically-downloadable corpus.

**Excluded near-misses.** Tor/network website-fingerprinting (traffic analysis), pure DNS/BGP/hardware/cellular/Bluetooth
work, and non-web LLM papers were filtered out to keep the corpus focused on the web attack/defense surface.

**"WEB-ADJACENT" verdicts** in the CSVs mark web-enabling infrastructure (web PKI/TLS, DNS-for-web, language runtimes)
whose core contribution is not itself a web attack surface; they are still placed in the most relevant topic.
