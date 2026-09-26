# Defensive-Papers (61 papers)

Detection, mitigation, hardening, and privacy/compliance defenses for the web.

Part of the [Web-Security Papers collection](../../README.md). Companion set: [Offensive-Papers](../Offensive-Papers/README.md).

## Topics

- **[Anti Tracking and Privacy Defenses](Anti-Tracking-and-Privacy-Defenses/)** (13) — Tracker/fingerprint detection and blocking, and privacy-preserving advertising mechanisms.
- **[Phishing and Scam Detection](Phishing-and-Scam-Detection/)** (10) — Detecting phishing and scam websites, including ML/LLM and reference-based detectors.
- **[Privacy Compliance and Consent](Privacy-Compliance-and-Consent/)** (10) — GDPR/CCPA compliance, cookie-consent and opt-out/GPC measurement and enforcement.
- **[Authentication and Passkey Defenses](Authentication-and-Passkey-Defenses/)** (8) — Passkeys/WebAuthn, account recovery, OAuth minimization, and SSO defenses.
- **[PKI and Transport Security](PKI-and-Transport-Security/)** (4) — Web PKI, certificate transparency, domain validation, and HSTS.
- **[Vulnerability Mitigation and Hardening](Vulnerability-Mitigation-and-Hardening/)** (4) — Runtime containment, SSRF/deserialization defenses, and hardening of web applications.
- **[Web Attack and Malware Detection](Web-Attack-and-Malware-Detection/)** (4) — Runtime detection of web attacks and analysis/deobfuscation of malicious JavaScript, plus web forensics.
- **[Web Agent and LLM Security](Web-Agent-and-LLM-Security/)** (3) — Defenses/benchmarks for web agents, prompt-injection resistance, and safe AI web search.
- **[Measurement Tools and SoK](Measurement-Tools-and-SoK/)** (2) — Reusable web-measurement infrastructure and systematization-of-knowledge on web methods.
- **[Supply Chain Security](Supply-Chain-Security/)** (2) — npm and multi-registry package supply-chain security.
- **[Content Protection and Anti Crawling](Content-Protection-and-Anti-Crawling/)** (1) — Protecting web content from unauthorized crawling and LLM scraping.

## Anti Tracking and Privacy Defenses (13)

- **FP-Fed Privacy-Preserving Federated Detection of Browser Fingerprinting** (NDSS 2024) — [PDF](https://www.ndss-symposium.org/wp-content/uploads/2024-360-paper.pdf) · `Anti-Tracking-and-Privacy-Defenses/NDSS-2024__Fp-Fed-Privacy-Preserving-Federated-Detection-Of-Browser-Fingerprinting.pdf`
- **Duumviri Detecting Trackers And Mixed Trackers With A Breakage Detector** (NDSS 2025) — [PDF](https://www.ndss-symposium.org/wp-content/uploads/2025-267-paper.pdf) · `Anti-Tracking-and-Privacy-Defenses/NDSS-2025__Duumviri-Detecting-Trackers-And-Mixed-Trackers-With-A-Breakage-Detector.pdf`
- **Block Cookies Not Websites Analysing Mental Models and Usability of the Privacy-Preserving Browser Extension CookieBlock** (PoPETs 2024) — [PDF](https://petsymposium.org/popets/2024/popets-2024-0012.pdf) · `Anti-Tracking-and-Privacy-Defenses/PoPETs-2024__Block-Cookies-Not-Websites-Analysing-Mental-Models-and-Usability-of-the-Privacy-Preserving.pdf`
- **Evaluating Google's Protected Audience Protocol** (PoPETs 2024) — [PDF](https://petsymposium.org/popets/2024/popets-2024-0147.pdf) · `Anti-Tracking-and-Privacy-Defenses/PoPETs-2024__Evaluating-Google-s-Protected-Audience-Protocol.pdf`
- **FP-tracer Fine-grained Browser Fingerprinting Detection via Taint-tracking and Entropy-based Thresholds** (PoPETs 2024) — [PDF](https://petsymposium.org/popets/2024/popets-2024-0092.pdf) · `Anti-Tracking-and-Privacy-Defenses/PoPETs-2024__FP-tracer-Fine-grained-Browser-Fingerprinting-Detection-via-Taint-tracking-and-Entropy-bas.pdf`
- **Summary Reports Optimization in the Privacy Sandbox Attribution Reporting API** (PoPETs 2024) — [PDF](https://petsymposium.org/popets/2024/popets-2024-0132.pdf) · `Anti-Tracking-and-Privacy-Defenses/PoPETs-2024__Summary-Reports-Optimization-in-the-Privacy-Sandbox-Attribution-Reporting-API.pdf`
- **The Devil is in the Details Detection Measurement and Lawfulness of Server-Side Tracking on the Web** (PoPETs 2024) — [PDF](https://petsymposium.org/popets/2024/popets-2024-0125.pdf) · `Anti-Tracking-and-Privacy-Defenses/PoPETs-2024__The-Devil-is-in-the-Details-Detection-Measurement-and-Lawfulness-of-Server-Side-Tracking-o.pdf`
- **Website Data Transparency in the Browser** (PoPETs 2024) — [PDF](https://petsymposium.org/popets/2024/popets-2024-0048.pdf) · `Anti-Tracking-and-Privacy-Defenses/PoPETs-2024__Website-Data-Transparency-in-the-Browser.pdf`
- **Beyond the Request: Harnessing HTTP Response Headers for Cross-Browser Web Tracker Detection** (PoPETs 2025) — [PDF](https://petsymposium.org/popets/2025/popets-2025-0007.pdf) · `Anti-Tracking-and-Privacy-Defenses/PoPETs-2025__Beyond-the-Request-Harnessing-HTTP-Response-Headers-for-Cross-Browser-Web-Tracker-Detection.pdf`
- **An Improved Entropy Measure for Web Browser Fingerprinting Risk** (PoPETs 2026) — [PDF](https://petsymposium.org/popets/2026/popets-2026-0102.pdf) · `Anti-Tracking-and-Privacy-Defenses/PoPETs-2026__An-Improved-Entropy-Measure-for-Web-Browser-Fingerprinting-Risk.pdf`
- **From Syntactic Matching to Taint Tracking and Back: A Comparative Study of Web Tracking Detection** (PoPETs 2026) — [PDF](https://petsymposium.org/popets/2026/popets-2026-0122.pdf) · `Anti-Tracking-and-Privacy-Defenses/PoPETs-2026__From-Syntactic-Matching-to-Taint-Tracking-and-Back-A-Comparative-Study-of-Web-Tracking-Detectio.pdf`
- **Arcanum Detecting and Evaluating the Privacy Risks of Browser Extensions on Web Pages and Web Content** (USENIX-Security 2024) — [PDF](https://www.usenix.org/system/files/usenixsecurity24-xie-qinge.pdf) · `Anti-Tracking-and-Privacy-Defenses/USENIX-Security-2024__Arcanum-Detecting-and-Evaluating-the-Privacy-Risks-of-Browser-Extensions-on-Web-Pages-and.pdf`
- **PURL Safe and Effective Sanitization of Link Decoration** (USENIX-Security 2024) — [PDF](https://www.usenix.org/system/files/usenixsecurity24-munir.pdf) · `Anti-Tracking-and-Privacy-Defenses/USENIX-Security-2024__PURL-Safe-and-Effective-Sanitization-of-Link-Decoration.pdf`

## Phishing and Scam Detection (10)

- **Scammagnifier Piercing The Veil Of Fraudulent Shopping Website Campaigns** (NDSS 2025) — [PDF](https://www.ndss-symposium.org/wp-content/uploads/2025-763-paper.pdf) · `Phishing-and-Scam-Detection/NDSS-2025__Scammagnifier-Piercing-The-Veil-Of-Fraudulent-Shopping-Website-Campaigns.pdf`
- **Ctphishcapture Uncovering Credential Theft Based Phishing Scams Targeting Cryptocurrency Wallets** (NDSS 2026) — [PDF](https://www.ndss-symposium.org/wp-content/uploads/2026-f2854-paper.pdf) · `Phishing-and-Scam-Detection/NDSS-2026__Ctphishcapture-Uncovering-Credential-Theft-Based-Phishing-Scams-Targeting-Cryptocurrency-Wallet.pdf`
- **LOKI Proactively Discovering Online Scam Websites by Mining Toxic Search Queries** (NDSS 2026) — [PDF](https://www.ndss-symposium.org/wp-content/uploads/2026-s184-paper.pdf) · `Phishing-and-Scam-Detection/NDSS-2026__Loki-Proactively-Discovering-Online-Scam-Websites-By-Mining-Toxic-Search-Queries.pdf`
- **PhishLang A Real-Time Fully Client-Side Phishing Detection Framework Using MobileBERT** (NDSS 2026) — [PDF](https://www.ndss-symposium.org/wp-content/uploads/2026-s1037-paper.pdf) · `Phishing-and-Scam-Detection/NDSS-2026__Phishlang-A-Real-Time-Fully-Client-Side-Phishing-Detection-Framework-Using-Mobilebert.pdf`
- **KnowPhish: Large Language Models Meet Multimodal Knowledge Graphs for Enhancing Reference-Based Phishing Detection** (USENIX-Security 2024) — [PDF](https://www.usenix.org/system/files/usenixsecurity24-li-yuexin.pdf) · `Phishing-and-Scam-Detection/USENIX-Security-2024__KnowPhish-Large-Language-Models-Meet-Multimodal-Knowledge-Graphs-for-Enhancing-Reference-B.pdf`
- **Less Defined Knowledge and More True Alarms: Reference-based Phishing Detection without a Pre-defined Reference List** (USENIX-Security 2024) — [PDF](https://www.usenix.org/system/files/usenixsecurity24-liu-ruofan.pdf) · `Phishing-and-Scam-Detection/USENIX-Security-2024__Less-Defined-Knowledge-and-More-True-Alarms-Reference-based-Phishing-Detection-without-a-P.pdf`
- **PhishDecloaker: Detecting CAPTCHA-cloaked Phishing Websites via Hybrid Vision-based Interactive Models** (USENIX-Security 2024) — [PDF](https://www.usenix.org/system/files/usenixsecurity24-teoh.pdf) · `Phishing-and-Scam-Detection/USENIX-Security-2024__PhishDecloaker-Detecting-CAPTCHA-cloaked-Phishing-Websites-via-Hybrid-Vision-based-Interac.pdf`
- **Evaluating the Effectiveness and Robustness of Visual Similarity-based Phishing Detection Models** (USENIX-Security 2025) — [PDF](https://www.usenix.org/system/files/usenixsecurity25-ji.pdf) · `Phishing-and-Scam-Detection/USENIX-Security-2025__Evaluating-the-Effectiveness-and-Robustness-of-Visual-Similarity-based-Phishing-Detection.pdf`
- **Designing Wallet-Based User Intervention for Approval Phishing Mitigation** (USENIX-Security 2026) — [PDF](https://www.usenix.org/system/files/usenixsecurity26-guan.pdf) · `Phishing-and-Scam-Detection/USENIX-Security-2026__Designing-Wallet-Based-User-Intervention-for-Approval-Phishing-Mitigation.pdf`
- **SoK: PHILTER: Uncovering Security and Functional Gaps in AI-based Phishing Website Detection Literature via an LLM-based Reasoning Framework** (USENIX-Security 2026) — [PDF](https://www.usenix.org/system/files/usenixsecurity26-alam.pdf) · `Phishing-and-Scam-Detection/USENIX-Security-2026__SoK-PHILTER-Uncovering-Security-and-Functional-Gaps-in-AI-based-Phishing-Website-Detection-Lite.pdf`

## Privacy Compliance and Consent (10)

- **A Large-Scale Study of Cookie Banner Interaction Tools and their Impact on Users Privacy** (PoPETs 2024) — [PDF](https://petsymposium.org/popets/2024/popets-2024-0002.pdf) · `Privacy-Compliance-and-Consent/PoPETs-2024__A-Large-Scale-Study-of-Cookie-Banner-Interaction-Tools-and-their-Impact-on-Users-Privacy.pdf`
- **Generalizable Active Privacy Choice Designing a Graphical User Interface for Global Privacy Control** (PoPETs 2024) — [PDF](https://petsymposium.org/popets/2024/popets-2024-0015.pdf) · `Privacy-Compliance-and-Consent/PoPETs-2024__Generalizable-Active-Privacy-Choice-Designing-a-Graphical-User-Interface-for-Global-Privac.pdf`
- **Johnny Still Can't Opt-out Assessing the IAB CCPA Compliance Framework** (PoPETs 2024) — [PDF](https://petsymposium.org/popets/2024/popets-2024-0120.pdf) · `Privacy-Compliance-and-Consent/PoPETs-2024__Johnny-Still-Can-t-Opt-out-Assessing-the-IAB-CCPA-Compliance-Framework.pdf`
- **Opted Out Yet Tracked Are Regulations Enough to Protect Your Privacy** (PoPETs 2024) — [PDF](https://petsymposium.org/popets/2024/popets-2024-0016.pdf) · `Privacy-Compliance-and-Consent/PoPETs-2024__Opted-Out-Yet-Tracked-Are-Regulations-Enough-to-Protect-Your-Privacy.pdf`
- **Johnny Can't Revoke Consent Either: Measuring Compliance of Consent Revocation on the Web** (PoPETs 2025) — [PDF](https://petsymposium.org/popets/2025/popets-2025-0133.pdf) · `Privacy-Compliance-and-Consent/PoPETs-2025__Johnny-Can-t-Revoke-Consent-Either-Measuring-Compliance-of-Consent-Revocation-on-the-Web.pdf`
- **Making Web Applications GDPR Compliant: A Comparative Evaluation of GDPR-Enforcement Frameworks** (PoPETs 2025) — [PDF](https://petsymposium.org/popets/2025/popets-2025-0157.pdf) · `Privacy-Compliance-and-Consent/PoPETs-2025__Making-Web-Applications-GDPR-Compliant-A-Comparative-Evaluation-of-GDPR-Enforcement-Frameworks.pdf`
- **Automated Large-Scale Analysis of Cookie Notice Compliance** (USENIX-Security 2024) — [PDF](https://www.usenix.org/system/files/usenixsecurity24-bouhoula.pdf) · `Privacy-Compliance-and-Consent/USENIX-Security-2024__Automated-Large-Scale-Analysis-of-Cookie-Notice-Compliance.pdf`
- **The Effect of Design Patterns on Present and Future Cookie Consent Decisions** (USENIX-Security 2024) — [PDF](https://www.usenix.org/system/files/usenixsecurity24-bielova.pdf) · `Privacy-Compliance-and-Consent/USENIX-Security-2024__The-Effect-of-Design-Patterns-on-Present-and-Future-Cookie-Consent-Decisions.pdf`
- **Navigating Cookie Consent Violations Across the Globe** (USENIX-Security 2025) — [PDF](https://www.usenix.org/system/files/usenixsecurity25-tang.pdf) · `Privacy-Compliance-and-Consent/USENIX-Security-2025__Navigating-Cookie-Consent-Violations-Across-the-Globe.pdf`
- **Websites' Global Privacy Control Compliance at Scale and over Time** (USENIX-Security 2025) — [PDF](https://www.usenix.org/system/files/usenixsecurity25-hausladen.pdf) · `Privacy-Compliance-and-Consent/USENIX-Security-2025__Websites-Global-Privacy-Control-Compliance-at-Scale-and-over-Time.pdf`

## Authentication and Passkey Defenses (8)

- **Post-quantum XML and SAML Single Sign-On** (PoPETs 2024) — [PDF](https://petsymposium.org/popets/2024/popets-2024-0128.pdf) · `Authentication-and-Passkey-Defenses/PoPETs-2024__Post-quantum-XML-and-SAML-Single-Sign-On.pdf`
- **SoK: Web Authentication and Recovery in the Age of End-to-End Encryption** (PoPETs 2025) — [PDF](https://petsymposium.org/popets/2025/popets-2025-0113.pdf) · `Authentication-and-Passkey-Defenses/PoPETs-2025__SoK-Web-Authentication-and-Recovery-in-the-Age-of-End-to-End-Encryption.pdf`
- **OAuthHub: Mitigating OAuth Data Overaccess through a Local Data Hub** (PoPETs 2026) — [PDF](https://petsymposium.org/popets/2026/popets-2026-0098.pdf) · `Authentication-and-Passkey-Defenses/PoPETs-2026__OAuthHub-Mitigating-OAuth-Data-Overaccess-through-a-Local-Data-Hub.pdf`
- **Secure Account Recovery for a Privacy-Preserving Web Service** (USENIX-Security 2024) — [PDF](https://www.usenix.org/system/files/usenixsecurity24-little.pdf) · `Authentication-and-Passkey-Defenses/USENIX-Security-2024__Secure-Account-Recovery-for-a-Privacy-Preserving-Web-Service.pdf`
- **Why Aren't We Using Passkeys Obstacles Companies Face Deploying FIDO2 Passwordless Authentication** (USENIX-Security 2024) — [PDF](https://www.usenix.org/system/files/usenixsecurity24-lassak.pdf) · `Authentication-and-Passkey-Defenses/USENIX-Security-2024__Why-Aren-t-We-Using-Passkeys-Obstacles-Companies-Face-Deploying-FIDO2-Passwordless-Authent.pdf`
- **Detecting Compromise of Passkey Storage on the Cloud** (USENIX-Security 2025) — [PDF](https://www.usenix.org/system/files/usenixsecurity25-islam.pdf) · `Authentication-and-Passkey-Defenses/USENIX-Security-2025__Detecting-Compromise-of-Passkey-Storage-on-the-Cloud.pdf`
- **Maybe there's only one passkey Challenges Investigating and Remediating Adversarial Passkeys** (USENIX-Security 2026) — [PDF](https://www.usenix.org/system/files/usenixsecurity26-daffalla.pdf) · `Authentication-and-Passkey-Defenses/USENIX-Security-2026__Maybe-there-s-only-one-passkey-Challenges-Investigating-and-Remediating-Adversarial-Passke.pdf`
- **The State of Passkeys: Studying the Adoption and Security of Passkeys on the Web** (USENIX-Security 2026) — [PDF](https://www.usenix.org/system/files/usenixsecurity26-jannett.pdf) · `Authentication-and-Passkey-Defenses/USENIX-Security-2026__The-State-of-Passkeys-Studying-the-Adoption-and-Security-of-Passkeys-on-the-Web.pdf`

## PKI and Transport Security (4)

- **Certificate Transparency Revisited The Public Inspections on Third-party Monitors** (NDSS 2024) — [PDF](https://www.ndss-symposium.org/wp-content/uploads/2024-834-paper.pdf) · `PKI-and-Transport-Security/NDSS-2024__Certificate-Transparency-Revisited-The-Public-Inspections-On-Third-Party-Monitors.pdf`
- **Ctng Secure Certificate And Revocation Transparency** (NDSS 2026) — [PDF](https://www.ndss-symposium.org/wp-content/uploads/2026-s213-paper.pdf) · `PKI-and-Transport-Security/NDSS-2026__Ctng-Secure-Certificate-And-Revocation-Transparency.pdf`
- **CoStricTor Collaborative HTTP Strict Transport Security in Tor Browser** (PoPETs 2024) — [PDF](https://petsymposium.org/popets/2024/popets-2024-0020.pdf) · `PKI-and-Transport-Security/PoPETs-2024__CoStricTor-Collaborative-HTTP-Strict-Transport-Security-in-Tor-Browser.pdf`
- **Cryptographically-Secured Domain Validation** (PoPETs 2026) — [PDF](https://petsymposium.org/popets/2026/popets-2026-0056.pdf) · `PKI-and-Transport-Security/PoPETs-2026__Cryptographically-Secured-Domain-Validation.pdf`

## Vulnerability Mitigation and Hardening (4)

- **Automatic Policy Synthesis and Enforcement for Protecting Untrusted Deserialization** (NDSS 2024) — [PDF](https://www.ndss-symposium.org/wp-content/uploads/2024-53-paper.pdf) · `Vulnerability-Mitigation-and-Hardening/NDSS-2024__Automatic-Policy-Synthesis-And-Enforcement-For-Protecting-Untrusted-Deserialization.pdf`
- **QUACK Hindering Deserialization Attacks via Static Duck Typing** (NDSS 2024) — [PDF](https://www.ndss-symposium.org/wp-content/uploads/2024-1015-paper.pdf) · `Vulnerability-Mitigation-and-Hardening/NDSS-2024__Quack-Hindering-Deserialization-Attacks-Via-Static-Duck-Typing.pdf`
- **SSRF vs Developers A Study of SSRF-Defenses in PHP Applications** (USENIX-Security 2024) — [PDF](https://www.usenix.org/system/files/usenixsecurity24-wessels.pdf) · `Vulnerability-Mitigation-and-Hardening/USENIX-Security-2024__SSRF-vs-Developers-A-Study-of-SSRF-Defenses-in-PHP-Applications.pdf`
- **Kintsugi: Empowering LLMs to Mitigate Web Vulnerabilities via Runtime Policy Injection** (USENIX-Security 2026) — [PDF](https://www.usenix.org/system/files/usenixsecurity26-peng-yihao.pdf) · `Vulnerability-Mitigation-and-Hardening/USENIX-Security-2026__Kintsugi-Empowering-LLMs-to-Mitigate-Web-Vulnerabilities-via-Runtime-Policy-Injection.pdf`

## Web Attack and Malware Detection (4)

- **Achieving Interpretable Dl Based Web Attack Detection Through Malicious Payload Localization** (NDSS 2026) — [PDF](https://www.ndss-symposium.org/wp-content/uploads/2026-s1029-paper.pdf) · `Web-Attack-and-Malware-Detection/NDSS-2026__Achieving-Interpretable-Dl-Based-Web-Attack-Detection-Through-Malicious-Payload-Localization.pdf`
- **From Obfuscated To Obvious A Comprehensive Javascript Deobfuscation Tool For Security Analysis** (NDSS 2026) — [PDF](https://www.ndss-symposium.org/wp-content/uploads/2026-f2198-paper.pdf) · `Web-Attack-and-Malware-Detection/NDSS-2026__From-Obfuscated-To-Obvious-A-Comprehensive-Javascript-Deobfuscation-Tool-For-Security-Analysis.pdf`
- **FV8 A Forced Execution JavaScript Engine for Detecting Evasive Techniques** (USENIX-Security 2024) — [PDF](https://www.usenix.org/system/files/usenixsecurity24-pantelaios.pdf) · `Web-Attack-and-Malware-Detection/USENIX-Security-2024__FV8-A-Forced-Execution-JavaScript-Engine-for-Detecting-Evasive-Techniques.pdf`
- **WEBRR A Forensic System for Replaying and Investigating Web-Based Attacks in The Modern Web** (USENIX-Security 2024) — [PDF](https://www.usenix.org/system/files/usenixsecurity24-allen.pdf) · `Web-Attack-and-Malware-Detection/USENIX-Security-2024__WEBRR-A-Forensic-System-for-Replaying-and-Investigating-Web-Based-Attacks-in-The-Modern-We.pdf`

## Web Agent and LLM Security (3)

- **WebSP-Eval: Evaluating Web Agents on Website Security and Privacy Tasks** (PoPETs 2026) — [PDF](https://petsymposium.org/popets/2026/popets-2026-0140.pdf) · `Web-Agent-and-LLM-Security/PoPETs-2026__WebSP-Eval-Evaluating-Web-Agents-on-Website-Security-and-Privacy-Tasks.pdf`
- **StruQ Defending Against Prompt Injection with Structured Queries** (USENIX-Security 2025) — [PDF](https://www.usenix.org/system/files/usenixsecurity25-chen-sizhe.pdf) · `Web-Agent-and-LLM-Security/USENIX-Security-2025__StruQ-Defending-Against-Prompt-Injection-with-Structured-Queries.pdf`
- **Unsafe LLM-Based Search Quantitative Analysis and Mitigation of Safety Risks in AI Web Search** (USENIX-Security 2025) — [PDF](https://www.usenix.org/system/files/usenixsecurity25-luo-zeren.pdf) · `Web-Agent-and-LLM-Security/USENIX-Security-2025__Unsafe-LLM-Based-Search-Quantitative-Analysis-and-Mitigation-of-Safety-Risks-in-AI-Web-Sea.pdf`

## Measurement Tools and SoK (2)

- **SoK State of the Krawlers Evaluating the Effectiveness of Crawling Algorithms for Web Security Measurements** (USENIX-Security 2024) — [PDF](https://www.usenix.org/system/files/usenixsecurity24-stafeev.pdf) · `Measurement-Tools-and-SoK/USENIX-Security-2024__SoK-State-of-the-Krawlers-Evaluating-the-Effectiveness-of-Crawling-Algorithms-for-Web-Secu.pdf`
- **Web Execution Bundles: Reproducible, Accurate, and Archivable Web Measurements** (USENIX-Security 2025) — [PDF](https://www.usenix.org/system/files/usenixsecurity25-hantke.pdf) · `Measurement-Tools-and-SoK/USENIX-Security-2025__Web-Execution-Bundles-Reproducible-Accurate-and-Archivable-Web-Measurements.pdf`

## Supply Chain Security (2)

- **From Noise To Signal Precisely Identify Affected Packages Of Known Vulnerabilities In Npm Ecosystem** (NDSS 2026) — [PDF](https://www.ndss-symposium.org/wp-content/uploads/2026-f1902-paper.pdf) · `Supply-Chain-Security/NDSS-2026__From-Noise-To-Signal-Precisely-Identify-Affected-Packages-Of-Known-Vulnerabilities-In-Npm-Ecosy.pdf`
- **DONAPI Malicious NPM Packages Detector using Behavior Sequence Knowledge Mapping** (USENIX-Security 2024) — [PDF](https://www.usenix.org/system/files/usenixsecurity24-huang-cheng.pdf) · `Supply-Chain-Security/USENIX-Security-2024__DONAPI-Malicious-NPM-Packages-Detector-using-Behavior-Sequence-Knowledge-Mapping.pdf`

## Content Protection and Anti Crawling (1)

- **Expshield Safeguarding Web Text From Unauthorized Crawling And Llm Exploitation** (NDSS 2026) — [PDF](https://www.ndss-symposium.org/wp-content/uploads/2026-f11-paper.pdf) · `Content-Protection-and-Anti-Crawling/NDSS-2026__Expshield-Safeguarding-Web-Text-From-Unauthorized-Crawling-And-Llm-Exploitation.pdf`
