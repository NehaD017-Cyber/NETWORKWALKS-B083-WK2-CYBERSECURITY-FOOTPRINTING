# NETWORKWALKS-B083-WK2-CYBERSECURITY-FOOTPRINTING-Reconnaissance
Hands-on Cybersecurity lab using Kali Linux to practice Foot-printing and Reconnaissance.

# Footprinting and Reconnaissance in Cybersecurity 

### After setting up the environmental virtual lab of VirtualBox and Kali Linux, we're going to learn and practice about Foot-printing and Reconnaissance in this project.

<!-- Lab & Environment Badges -->
![Skill](https://img.shields.io/badge/Skill-Cybersecurity-D32F2F?style=for-the-badge)
![Skill](https://img.shields.io/badge/Skill-Ethical%20Hacking-F57C00?style=for-the-badge)
![Skill](https://img.shields.io/badge/Skill-Footprinting-388E3C?style=for-the-badge)
![Lab](https://img.shields.io/badge/Lab-Virtual%20Lab-1976D2?style=for-the-badge)
<!-- Platform & Environment -->
![VirtualBox](https://img.shields.io/badge/VirtualBox-v7.2-0078D4?style=for-the-badge&logo=virtualbox&logoColor=white)
![Kali Linux](https://img.shields.io/badge/Kali_Linux-v2026.2-FF6F00?style=for-the-badge&logo=kalilinux&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-Repository-181717?style=for-the-badge&logo=github&logoColor=white)
<!-- Tools & Frameworks -->
![whois](https://img.shields.io/badge/Tool-whois-7B1FA2?style=for-the-badge)
![WhatWeb](https://img.shields.io/badge/Tool-WhatWeb-E91E63?style=for-the-badge)
![wafw00f](https://img.shields.io/badge/Tool-wafw00f-009688?style=for-the-badge)
![curl -I](https://img.shields.io/badge/Command-curl%20--I-008080?style=for-the-badge)
![nslookup](https://img.shields.io/badge/Command-nslookup-9C27B0?style=for-the-badge)
![DNS Lookup](https://img.shields.io/badge/Command-DNS%20Lookup-4CAF50?style=for-the-badge)
![IP Address](https://img.shields.io/badge/Command-IP%20Address-FF5722?style=for-the-badge)

![Reconnaissance](https://img.shields.io/badge/Command-Reconnaissance-4CAF50?style=for-the-badge)
![GHDB](https://img.shields.io/badge/Tool-GHDB-D32F2F?style=for-the-badge)
![theHarvester](https://img.shields.io/badge/Tool-theHarvester-FF6F00?style=for-the-badge)
![Zenmap](https://img.shields.io/badge/Tool-Zenmap-1976D2?style=for-the-badge)
![Maltego](https://img.shields.io/badge/Tool-Maltego-7B1FA2?style=for-the-badge)

Isolated virtual lab for practicing Cybersecurity, Ethical Hacking, Footprinting and Reconnaissance.

## 🔎 Project Overview:

The first project was about doing environmental set-up of the virtual lab VirtualBox and Kali Linux. So, in this project we'll learn about Footprinting and Reconnaissance, that is the first step in the Cybersecurity. In this project we will use multiple tools of Kali, GHDB, Maltego, the Harvester, Zenmap and many others. 

---

# Project-Module 1
   Footprinting and Reconnaissance attacks with multiple Kali tools.

## 🔐 Objectives:

Step 1: Run 'whois' to find the registration details of the domain you are using for the project.

Step 2: Run 'whatweb' to fingerprint the web technologies.

Step 3: Run 'nslookup' to resolve the domain to its IP address.

Step 4: Run 'curl -I' to read the HTTP response headers.

Step 5: Run 'wafw00f' to detect a Web Application Farewall.

Step 6: Run 'dnsrecon' to enumerate all DNS records.

--

### Step 1: 

* Open the Kali Linux terminal and run the following command:
  
```bash
  whois <domain>
```

The whois command is an open-source network administration tool used to query database records for domain names and IP addresses. It helps you gather detailed background intelligence (footprinting) about a target website or server.

<img width="1910" height="940" alt="whois networkwalks com" src="https://github.com/user-attachments/assets/466c382e-a7e4-4794-b049-d8d7cef526e4" />

### Step 2: 

* Open the Kali Linux terminal and run the following command:

```bash
whatweb <domain>
```

The whatweb command is a web scanner used in footprinting to identify the technologies running on a website (such as CMS platform, web server type, IP address, embedded scripts, and HTTP status codes).



### Step 3: 

* Open the Kali Linux terminal and run the following command: 

```bash
nslookup <domain>
```

The nslookup (Name Server Lookup) command is a network administration tool used for querying Domain Name System (DNS) servers to find IP addresses associated with a domain name, or vice versa.



### Step 4:

* Open the Kali Linux terminal and run the following command:

  ```bash
  curl -I https://<domain>
  ```

  The command curl -I (or curl --head) is used in cybersecurity footprinting and web debugging to fetch only the HTTP response headers from a target web server, without downloading the entire website page body (HTML, CSS, images).

<img width="1910" height="940" alt="curl networkwalks com" src="https://github.com/user-attachments/assets/c27e2eb4-eae8-426a-b956-9ee1f99a1e53" />

### Step 5:

* Open the Kali Linux and run the following command:

```bash
wafw00f <domain>
```

The command wafw00f (often pronounced/written as "WAF00F") is an open-source command-line tool used in cybersecurity footprinting and reconnaissance to identify and fingerprint Web Application Firewalls (WAFs) protecting a website.




### Step 6: 

* Open the Kali Linux and run the following command:

  ```bash
  dnsrecon -d <domain>
  ```
  
The command dnsrecon is a powerful Python-based DNS enumeration tool used during the reconnaissance and footprinting phase of a penetration test. It helps discover subdomains, zone transfers, DNS records, and hidden network infrastructure associated with a target domain.

---

## 🧠 What I Learned:

In this lab, I gained hands-on experience using Kali Linux tools in footprinting and reconnaissance to map domain assets, web technologies, and DNS infrastructure.

* Command Breakdown:
  
1. whois:

Extracted domain registration details, owner contact information, registrar data, and name server locations.

2. nslookup:

Performed forward and reverse DNS queries to resolve domain names to IP addresses and identify name servers.

3. curl -I:

Fetched raw HTTP response headers to inspect server types, status codes, and security policies without loading the webpage body.

4. whatweb:

Fingerprinted target websites to discover Content Management Systems (CMS), web frameworks, and backend scripts.

5. wafw00f: 

Identified active Web Application Firewalls (WAF) such as Cloudflare or AWS WAF protecting the web application.

6. dnsrecon:

Enumerated DNS records (A, MX, NS, TXT), checked for AXFR zone transfer vulnerabilities, and mapped subdomains.

---

# Project-Module 2
  Footprinting and Reconnaissance with the help of Google Hacking DataBase.

 ## 🔏 Objectives:

 Step 1: Open the Exploit Database, go to the GHDB (Google Hacking Database).
 
 Step 2: Go to the Quick search and search cam.
 
 Step 3: From the showed-up dorks, select any and copy it and search it in Google.
 
 Step 4: Open the visible site to get the live vulnerability security camera and IP address.

 Step 5: Select listings of downloadable mathematics ebooks in pdfs from the Exploit Database and search them in google search bar too.

 Step 6: List any 10 of them in the table.

---

### Step 1:

   Open Exploit Database and go to GHDB.

<img width="640" height="376" alt="Screenshot 2026-09-16 184420" src="https://github.com/user-attachments/assets/45121ad0-1203-47c1-94dd-3131c140ef2b" />

### Step 2:

Search cam on the Quick Search.

<img width="639" height="375" alt="Screenshot 2026-09-16 203206" src="https://github.com/user-attachments/assets/bdb9dd46-21d3-41bb-aed4-d6e37f3d71d6" />

### Step 3: 

Get Vulnerability Security Camera and IP Address.

<img width="491" height="376" alt="Screenshot 2026-09-16 213214" src="https://github.com/user-attachments/assets/de20ef72-14d8-42b6-aec0-2066e3aeef31" />

<img width="640" height="374" alt="Screenshot 2026-09-16 213154" src="https://github.com/user-attachments/assets/330385c2-b32f-4713-b15c-7fd0c976ef1d" />

<img width="640" height="378" alt="Screenshot 2026-09-16 201809" src="https://github.com/user-attachments/assets/34c2bd8a-d097-4627-9997-7c759e820275" />

<img width="640" height="371" alt="Screenshot 2026-09-16 201508" src="https://github.com/user-attachments/assets/f923ef35-217a-4347-953d-99f401ac405e" />

| No. | Link | Relevant Dork | Username / Password |
| :--- | :--- | :--- | :--- |
| **01** | `http://217.155.202.203:8088/` | `intitle:"ContaCam" "Snapshot Image"` | - |
| **02** | `http://109.164.108.255:8090/` | `intitle:"Milesight Network Camera" intext:"Language"` | - |
| **03** | `http://109.233.191.130:8080/` | `intitle:"webcamxp 5" intext: "live stream"` | - |
| **04** | `http://50.184.100.114:8000/` | `intitle:"NetCamSC*"` | - |
| **05** | `http://109.164.203.165/` | `"Camera Live Image" inurl:"guestimage.html"` | - |
| **06** | `http://99.114.240.169:8080/` | `intitle:"Webcam" inurl:WebCam.htm` | - |
| **07** | `http://66.206.54.197/` | `Display Cameras intitle:"Express6 Live Image"` | - |
| **08** | `http://79.157.102.84:82/` | `intitle:"INTELLINET" intitle:"IP Camera Homepage"` | - |
| **09** | `http://208.107.246.94` | `inurl:control/camerainfo` | - |
| **10** | `http://62.49.17.87:8000` | `intitle:"NetCam Live Image" -.edu -.gov -johnny.ihackstuff.com` | - |

### Step 4: 

Get Mathematics ebooks pdfs.


| No. | Link | Relevant Dork | Username / Password |
| :--- | :--- | :--- | :--- |
| **01** | `https://www.math.dartmouth.edu.carip.pdf` | `intitle:"index of /" mathematics pdf` | - |
| **02** | `https://vps.uttarahumara.edu.mx` | `intitle:"index of" "parent directory" "math" filetype:pdf` | - |
| **03** | `https://www.academia.edu` | `intitle:"index of /math/" "calculus" / "algebra"` | - |
| **04** | `https://jaem.isikun.edu.tr.articles.vol.12no.2` | `intitle:"index of /" "mathematics" filetype:pdf` | - |
| **05** | `https://nyjm.albany.edu` | `intitle:"index of" (calculus / algebra / topology / statistics) filetype:pdf` | - |
| **06** | `https://public.csusm.edu.research` | `site:edu intitle:"index of" "mathematics" filetype:pdf` | - |
| **07** | `https://jontalle.web.engr.illinois.edu > uploads` | `intitle:"index of /ebooks" "mathematics" filetype:pdf` | - |
| **08** | `https://annalsmcs.org › amcs › article` | `(site:gov / site:org) intitle:"index of" "mathematics" filetype:pdf` | - |
| **09** | `https://ftp.yz.yamagata-u.ac.jp > pub` | `"Apache" / "nginx" intitle:"index of /" "mathematics" "size"` | - |
| **10** | `https://lordsuniversal.edu.in` | `inurl:/wp-content/uploads/ "mathematics" filetype:pdf` | - |








































  
