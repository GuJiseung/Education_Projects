# Why Naver Bug Bounty?
- This Project was initiated during the K-Shield Jr. program.
- We wanted to evaluate our growth by attempting a real bug bounty program.
- Bug bounties are known for high difficulty, so we aimed to test our vulnerability assessment and pentesting skills.

# Objectives
- Attempt to discover at least one vulnerability such as XSS, SQL Injection, or SSRF etc.
- Use the experience as motivation to improve if no results were achieved.

# Tools Used
- **Kali Linux** - Used as our main penetration testing OS.
- **Nikto** - Collected IP and port information of the target.
- **WhatWeb** - Gathered summary information of the target website.
- **Python** - Crawled "Naver Pay" and related services to analyze source code.
- **DNSdumpster** - Enumerated subdomains for additional attack surface analysis.
- **BurpSuite** - Intercepted and manipulated traffic to test various vulnerabilities.

# Scenario Design
- Two scenarios were designed and executed in pairs.

### [Scenario 1]
Attempt to extract personal information such as delivery or reservation details from "Naver Pay".

### [Scenario 2]
Attemp to exploit vulnerabilities in event/coupon features to steal information or redirect to malicious pages.

#  Process & Results
### [Information Gathering]
\- Performed Nikto scanning to obtain Naver Pay's IP and port information.
<img width="808" height="494" alt="image" src="https://github.com/user-attachments/assets/71887f5c-0b35-4886-a02d-eb9d1f0e5189" />

<br>- Used WhatWeb to extract website metadata.
<img width="824" height="210" alt="image" src="https://github.com/user-attachments/assets/17a94386-417d-45ad-9997-74027ac0264b" />

<br>- Crawled related services to inspect source code.
<img width="660" height="630" alt="image" src="https://github.com/user-attachments/assets/43faba2a-0c7e-4001-a9a3-53e67bf31492" />
<img width="824" height="567" alt="image" src="https://github.com/user-attachments/assets/eb2cc356-5db3-4c56-a766-ab960f6d63cb" />

<br>- Enumerated subdomains using DNSdumpster.
<img width="650" height="558" alt="image" src="https://github.com/user-attachments/assets/99e7cf9e-cdab-4700-bd9b-2b9f3ad3ae17" />

<br>**[-] No meaningful vulnerabilities were found.**

### [Vulnerability Assessment]
\- Used BurpSuite to test for SQL Injection, SSRF, and other vulnerabilities.
<img width="797" height="448" alt="image" src="https://github.com/user-attachments/assets/b687f8fe-e0a2-46d5-8165-2a40ae741285" />


**[-] No exploitable vulnerabilities were identified.**

### [Final Outcome]
- Both scenarios resulted in no findings.
- Due to limited time in the final project schedule, further testing was not possible.
- We realized the need to enhance our vulnerability assessment skills.
- Decided to revisit bug bounty challenges after further improvement.
