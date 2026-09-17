no# NETWORKWALKS-B083-WK2-CYBERSECURITY-FOOTPRINTING-RECONNAISSANCE
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
   FOOTPRINTING AND RECONNAISSANCE WITH THE KALI TOOLS.

## 📌 Objectives:

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

<img width="320" height="152" alt="Screenshot 2026-09-17 151456" src="https://github.com/user-attachments/assets/f534883d-6d2c-40cf-ae1c-423ff31e040c" />

### Step 3: 

* Open the Kali Linux terminal and run the following command: 

```bash
nslookup <domain>
```

The nslookup (Name Server Lookup) command is a network administration tool used for querying Domain Name System (DNS) servers to find IP addresses associated with a domain name, or vice versa.

<img width="1910" height="940" alt="nslookup networkwalks com" src="https://github.com/user-attachments/assets/33419f36-e032-4e41-89d0-82d8ba518623" />

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

<img width="1600" height="787" alt="wafw00f" src="https://github.com/user-attachments/assets/1c947c5a-bb88-410a-931e-ae4c98b1e65d" />

### Step 6: 

* Open the Kali Linux and run the following command:

  ```bash
  dnsrecon -d <domain>
  ```
  
The command dnsrecon is a powerful Python-based DNS enumeration tool used during the reconnaissance and footprinting phase of a penetration test. It helps discover subdomains, zone transfers, DNS records, and hidden network infrastructure associated with a target domain.

---

## ♟️Command Breakdown:

In this lab, I gained hands-on experience using Kali Linux tools in footprinting and reconnaissance to map domain assets, web technologies, and DNS infrastructure.
  
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
  FOOTPRINTING AND RECONNAISSANCE WITH THE HELP OF GOOGLE HACKING DATABASE.
 ## 📌 Objectives:

 Step 1: Open the Exploit Database, go to the GHDB (Google Hacking Database).
 
 Step 2: Go to the Quick search and search cam.
 
 Step 3: From the showed-up dorks, select any and copy it and search it in Google.
 
 Step 4: Open the visible site to get the live vulnerability security camera and IP address.

 Step 5: Select listings of downloadable mathematics ebooks in pdfs from the Exploit Database and search them in google search bar too.

 Step 6: List any 10 of them in the table.

---

### Step 1:

* Open Exploit Database and go to GHDB.

<img width="640" height="376" alt="Screenshot 2026-09-16 184420" src="https://github.com/user-attachments/assets/45121ad0-1203-47c1-94dd-3131c140ef2b" />

### Step 2:

* Search cam on the Quick Search.

<img width="639" height="375" alt="Screenshot 2026-09-16 203206" src="https://github.com/user-attachments/assets/bdb9dd46-21d3-41bb-aed4-d6e37f3d71d6" />

### Step 3: 

* Get Vulnerability Security Camera and IP Address.

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

* Get downloadable Mathematics eBooks pdfs from relevant dorks. 

<img width="640" height="375" alt="Screenshot 2026-09-16 193257" src="https://github.com/user-attachments/assets/7971cde4-ea27-4455-8c2a-36cbc04ec367" />

| No. | Link | Relevant Dork | Username / Password |
| :--- | :--- | :--- | :--- |
| **01** | `https://sajaipuriacollege.ac.in/pdf/pdf/MATHEMATICS/` | `intitle:"index of /" mathematics pdf` | - |
| **02** | `https://www.math.ksu.edu/~dbski/writings/further.pdf` | `site:.gov OR site:.edu "mathematics textbook" filetype:pdf` | - |
| **03** | `https://www.jsoftware.com/books/pdf/` | `intitle:"index of /" "epub" OR "pdf" "calculus" OR "algebra"` | - |
| **04** | `https://jaem.isikun.edu.tr/web/images/articles/vol.12.no.2/23.pdf` | `intitle:"index of /" "mathematics" filetype:pdf` | - |
| **05** | `https://arxiv.org/pdf/2608.28796` | `intitle:"index of" (calculus / algebra / topology / statistics) filetype:pdf` | - |
| **06** | `https://nyjm.albany.edu/j/1995/1-9.pdf` | `site:edu intitle:"index of" "mathematics" filetype:pdf` | - |
| **07** | `https://math.colgate.edu/~integers/w58/w58.pdf` | `site:.edu intitle:"index of" "math" + "books" filetype:pdf` | - |
| **08** | `https://www.cs.ucdavis.edu/~rogaway/classes/20/fall21/mit-book.pdf` | `site:.edu inurl:courses "calculus" filetype:pdf` | - |
| **09** | `https://ftp.yz.yamagata-u.ac.jp/pub/linux/gentoo/sci-mathematics/mathematica/` | `"Apache" / "nginx" intitle:"index of /" "mathematics" "size"` | - |
| **10** | `https://antinifizicari.wordpress.com/wp-content/uploads/2019/08/basic-mathematics-for-college-students-pdfdrive.com-.pdf` | `inurl:/wp-content/uploads/ "mathematics" filetype:pdf` | - |

---

## 🗝️ Key Concepts
Passive Reconnaissance: Because you are searching through Google's index rather than connecting directly to a website, the target organization receives no direct traffic from you and cannot detect the search in their server logs.

## 🪢 Dual-Use Tool:

* Attackers use dorks to locate exposed login portals, open directories, database backups, configuration files, and unsecured devices (like security cameras).

* Defenders use the same search terms on their own domains to find exposed files and remove or secure them before they are exploited.

---

# Project-Module 3

FOOTPRINTING WITH MALTEGO.
## 📌 Objectives:

Step 1: Download & install Maltego on a Windows Computer.

Step 2: Find all email addresses related to the target organization
domain networkwalks.com (with due permission)

---

### Step 1:

* Open the website https://maltego.com and download Maltego:

<img width="640" height="374" alt="Screenshot 2026-09-17 103237" src="https://github.com/user-attachments/assets/88f9bd78-b27d-4af5-a91d-c9189772d694" />

<img width="640" height="367" alt="Screenshot 2026-09-17 103349" src="https://github.com/user-attachments/assets/5d7e0acd-3663-4d14-b281-52b7a321b55c" />

* Run Maltego setup & install it:

<img width="632" height="248" alt="Screenshot 2026-09-17 103601" src="https://github.com/user-attachments/assets/992b5bdd-38af-4284-81ac-bfea3f79f530" />

<img width="452" height="291" alt="Screenshot 2026-09-17 103737" src="https://github.com/user-attachments/assets/2ee32a24-8fe5-46ca-af1b-c318883983f5" />

<img width="640" height="374" alt="Screenshot 2026-09-17 103703" src="https://github.com/user-attachments/assets/0b45eb62-08ce-4297-93b8-3248fa2c0764" />

<img width="640" height="374" alt="Screenshot 2026-09-17 103921" src="https://github.com/user-attachments/assets/c5d27b0a-1b65-43b6-9255-e32c867babea" />
<img width="640" height="377" alt="Screenshot 2026-09-17 103814" src="https://github.com/user-attachments/assets/1de721e7-fa34-4622-8ea0-54a28347e73b" />

* Run Maltego after installation & complete the configuration:

<img width="640" height="373" alt="Screenshot 2026-09-17 104547" src="https://github.com/user-attachments/assets/839fea8e-a6a1-4dba-8abe-76f4ceb66eb4" />

<img width="571" height="338" alt="Screenshot 2026-09-17 104648" src="https://github.com/user-attachments/assets/d56e75db-2883-4512-877b-e1ed7b4f5eac" />

* Fill the registration form and Create your Maltego ID:

<img width="632" height="360" alt="Screenshot 2026-09-17 104715" src="https://github.com/user-attachments/assets/9cda192c-a90a-433a-9dae-7fb40fa06888" /> 

* Complete the Authentication and start Maltego: 

<img width="572" height="338" alt="Screenshot 2026-09-17 105900" src="https://github.com/user-attachments/assets/dd5485a4-c3ae-4d38-ade0-44be46e3f41c" />

<img width="640" height="374" alt="Screenshot 2026-09-17 110114" src="https://github.com/user-attachments/assets/3ad58deb-4890-4a71-b0bc-f99747120f96" />

* Maltego is now ready to run transforms.

### Step 2:

* Search for “Domain” & drag to main area:

Double-click on the entity & change name to networkwalks.com.

<img width="640" height="373" alt="Screenshot 2026-09-17 110445" src="https://github.com/user-attachments/assets/7a88e3d6-b725-4d5e-963f-f5dcb9ce3340" />

* Right-click & filter for email related transforms & run it:

<img width="640" height="371" alt="Screenshot 2026-09-17 113030" src="https://github.com/user-attachments/assets/6f1cef60-8f09-40af-b057-0fba1bb95105" />

The email addresses related to networkwalks.com have been harvested now.

* To website mentioning domains:

<img width="639" height="380" alt="Screenshot 2026-09-17 113109" src="https://github.com/user-attachments/assets/e08051ce-ca9f-4581-989d-5dfbb5b7b801" />

## ❔ Why Maltego?

* Maltego is a graphical link-analysis and Open-Source Intelligence (OSINT) tool used to gather information and visually map out relationships between data points on the internet.

* Instead of reading raw logs or text-based search results, Maltego connects pieces of information—like domain names, IP addresses, email addresses, social media profiles, and company networks—into an interactive visual graph.

---

# Project-Module 4

FOOTPRINTING & RECONNAISSANCE
WITH theHARVESTER

## 📌 Objectives:

Step 1: Find email IDs & sub-domains related to a target organization <domain>
using the theHarvester tool in Kali Linux with Baidu. Set the limit of number of
results to 1000.

Step 2: Find email IDs & sub-domains related to a target organization <domain>
using the theHarvester tool in Kali Linux with all sources. Set the limit of number of
results to 50.

---

### Step 1:

* Open theHarvester tool in Kali Linux from the applications.

Read the usage instructions & guidelines.

<img width="1910" height="940" alt="theHarvester" src="https://github.com/user-attachments/assets/e238d070-76c2-49b6-8306-fb4497c1207b" />

* Usage: theHarvester [-h] -d DOMAIN [-l LIMIT] [-S START] [-p] [-s] [--screenshot SCREENSHOT] [-e DNS_SERVER] [-t] [-r [DNS_RESOLVE]] [-n] [-c] [-f FILENAME] [-w WORDLIST] [-a] [-q] [-b SOURCE]

theHarvester is used to gather open source intelligence (OSINT) on a company or domain.

* In the terminal windows, type below command to start theHarvester & search for the required detail using Baidu:

```bash
$ theHarvester -d microsoft.com -l 1000 -b baidu
```

### Step 2:

* In the terminal windows, type below command to start theHarvester & search for the required detail using all:

``` bash
$ theHarvester -d microsoft.com -l 50 -b all
```

<img width="1910" height="940" alt="the harvestre microsoft com" src="https://github.com/user-attachments/assets/3136024e-674a-40fe-a544-ff3ed0334a67" />

---

## ⁉️ What It Collects:

* Email Addresses: Finds leaked or published employee emails associated with a domain.

* Subdomains & Hostnames: Discovers subdomains (e.g., admin.example.com, vpn.example.com).

* IP Addresses: Maps gathered subdomains to their corresponding public IP addresses.

* Employee Names: Scrapes names and titles from platforms like LinkedIn for social engineering risk analysis.

* Open Ports & Virtual Hosts: Identifies active services exposed to the public internet.

---

# Project-Module 5

NETWORK SCANNING WITH ZENMAP

* Nmap (Network Mapper) is an open-source command-line tool used for network discovery, port scanning, and vulnerability auditing. It sends custom IP packets to a target to determine what devices are active and what services they run.
  
## 📌 Objectives:

Step 1: Download & install Zenmap from official website on your Windows PC.

Step 2: Find your local IP address & your LAN subnet.

Step 3: Find the list of live hosts/PC’s in your IP subnet.

Step 4: Display & save the output topology in PDF Format on your desktop.

---

### Step 1:

* Download & install Zenmap from official website on your Windows PC:

``` bash
https://nmap.org/download.html
```

<img width="640" height="374" alt="Screenshot 2026-09-17 125618" src="https://github.com/user-attachments/assets/b0f5742f-5dea-4dc4-8bb4-100cae0ef2e0" />

### Step 2:

* Find your local IP address & your LAN subnet:

Open CMD & run ipconfig command to find your PC’s local IP address &
your local LAN subnet:

<img width="640" height="376" alt="Screenshot 2026-09-17 125722" src="https://github.com/user-attachments/assets/9b83d0cc-1437-481d-a653-1035ec9936bd" />

### Step 3:

* Find the list of live hosts/PC’s in your IP subnet:

Open Zenmap, input the local LAN subnet & select Ping Scan to find the list of
live hosts in your subnet:

<img width="640" height="376" alt="Screenshot 2026-09-17 144728" src="https://github.com/user-attachments/assets/879c4de0-c9dc-44de-8298-e24755f0a39f" />

* Click on Topology, turn on legend, read the legend in detail & click on Save
Graphic:

<img width="640" height="377" alt="Screenshot 2026-09-17 144858" src="https://github.com/user-attachments/assets/a7492135-43c2-49bc-a6ff-6c0197cc8b77" />

### Step 4:

* Display & save the output topology in PDF Format on your desktop:

<img width="640" height="371" alt="Screenshot 2026-09-17 141332" src="https://github.com/user-attachments/assets/6e08653a-a767-4f68-bf3d-564562875b36" />

Select PDF from the list.

The PDF file will be saved on your desktop.

Save the topology PDF and include it in your final report.

<img width="581" height="357" alt="Screenshot 2026-09-17 150213" src="https://github.com/user-attachments/assets/9b4f3039-be89-46f1-a960-9128ac8164ce" />

---

## 🧠 What I learned:

* Installation & Driver Setup:

 How to install Zenmap on Windows along with Npcap (the raw packet capture driver needed for network scanning).

* Subnet Discovery:

   How to convert an IP address (192.168.1.x) and Subnet Mask (255.255.255.0) into CIDR notation (192.168.1.0/24) to target an entire local network.

* Ping Scanning (-sn):

  How to run a light sweep across a network segment to detect active (live) systems without performing full port scans.

* Topology Visualization:

   How to read interactive node graphs showing hops/connections between host devices and export visual topology maps for reporting.

---

# Project-Report-Final

PENETRATION TESTING REPORT

| Pentester Name (Cybersecurity Professional) | NEHA |
| :--- | :--- |
| **Program/Batch** | B083-Networkwalks |
| **Date** | 17 September 2026 |
| **Modules completed** | W2-PM1 (Multiple Kali Tools)<br>W2-PM5 (Zenmap Scanning) |
| **Client/Target** | 1. Networkwalks (secured written permission already)<br>2. My own local LAN Network |
| **Permission secured from client?** | Yes |
| **Phases covered** | **Phase 1:** Reconnaissance & Footprinting<br>**Phase 2:** Scanning & Network Discovery<br>**Phase 3-5:** In Progress |

---

## 💣 Disclaimer and Liability:

* The activities documented in this repository were performed strictly on systems and devices where explicit, written permission was secured, or on hardware owned directly by the author.

* All content, commands, and materials presented here are provided solely for educational and research purposes.
Lawful Use Only: Do not use any information or code from this project to engage in unauthorized access or illegal activities.

* No Liability:

 The authors, instructors, and Networkwalks assume no liability for any actions taken or misuse of the information provided herein.

* Individual Responsibility: 

You are entirely responsible for your own actions. Misuse of cyber security tools and techniques can lead to severe criminal charges and legal penalties.

---

## 🔭 Tools used and Methodologies:

| Tool Name | Tool Type / Category | Primary Purpose & Usage |
| :--- | :--- | :--- |
| **Whois** | Information Gathering / OSINT | Queries registrar databases to retrieve domain registration, ownership details, IP ranges, and technical contacts. |
| **WhatWeb** | Web Reconnaissance | Scans websites to identify server technologies, CMS platforms, embedded scripts, and HTTP headers. |
| **NSlookup** | DNS Diagnostics | Interrogates DNS servers to resolve domain names to IP addresses and query specific DNS records (A, MX, NS). |
| **curl -I** | Web Inspection | Fetches HTTP/HTTPS response headers from a web server without downloading the page body to inspect server banners and security settings. |
| **DNSrecon** | DNS Enumeration | Automates DNS reconnaissance, executing zone transfers, cache snooping, and subdomain brute-forcing. |
| **Zenmap** | Network Discovery (GUI) | Graphical frontend for Nmap used to scan open ports, detect operating systems, and visualize network topology graphs. |
| **Maltego** | Graphical OSINT / Data Mining | Interactive link-analysis tool used to map and visualize relationships between domains, IP addresses, networks, and infrastructure. |
| **GHDB (Google Hacking Database)** | OSINT Resource | A compiled database of advanced search queries (Google Dorks) used to discover sensitive information and exposed web assets. |
| **theHarvester** | OSINT / E-mail Harvesting | Gathers subdomains, hostnames, employee names, open ports, and email addresses from public search engines and PGP key servers. |

---

## 💻 Activities Performed:

In this phase of the lab, two primary cybersecurity procedures were executed:

* **Footprinting & Reconnaissance:** Active and passive intelligence gathering was conducted using Kali Linux tools. Registrations and administrative details were collected using `whois`, while domain records were queried using `nslookup`. DNS infrastructure was enumerated with `dnsrecon`. Web target analysis was performed using `whatweb` to identify underlying frameworks, `curl -I` to inspect raw HTTP response headers, and `wafw00f` to detect active Web Application Firewalls.
* **Network Scanning & Discovery:** Subnet host discovery was performed using `Zenmap` across the `192.168.56.0/24` network segment. The scan successfully identified three live hosts on the network: the virtual gateway (`192.168.56.1`), the target system (`192.168.56.100`), and the local Kali Linux attacker machine (`192.168.56.101`).

---

## 🦂 Risk Analysis:

| Module / Tool | Focus Area | Identified Risk & Operational Impact |
| :--- | :--- | :--- |
| **Module 1: Kali Linux Reconnaissance Tools** *(Whois, WhatWeb, NSlookup, cURL, Wafw00f, DNSrecon)* | Active & Passive Footprinting | **Low to Medium Risk:** Exposes administrative contacts, DNS records, web server banners, and backend framework versions. Threat actors can use this intelligence to craft targeted exploits or bypass Web Application Firewalls (WAF). |
| **Module 2: Google Hacking Database (GHDB)** | OSINT & Search Engine Dorking | **Medium Risk:** Uncovers publicly indexed sensitive files, exposed admin login portals, backup archives, and configuration flaws without directly interacting with or alerting the target server. |
| **Module 3: Maltego** | Link Analysis & Entity Mapping | **Medium Risk:** Maps complex relationships across domain infrastructures, IP blocks, MX servers, and personnel data. Allows adversaries to visually identify single points of failure or optimal entry points across the network topology. |
| **Module 4: theHarvester** | OSINT / Email & Subdomain Harvesting | **Medium to High Risk:** Gathers internal hostnames, active subdomains, and corporate email addresses from public databases. This data fuels highly convincing spear-phishing campaigns and password-spraying attacks. |
| **Module 5: Zenmap / Nmap Scanner** | Active Network & Port Scanning | **High Risk:** Direct host discovery on target `192.168.56.100` reveals open ports, running services, and OS signatures. Unrestricted visibility gives attackers the exact blueprint needed to launch targeted exploitation attempts. |

---

## 🎓 Recommendations & Countermeasures:

| Module / Vector | Recommended Mitigation Strategy | Implementation Action |
| :--- | :--- | :--- |
| **Footprinting & OSINT** *(Whois, theHarvester, GHDB)* | **Information Disclosure Minimization** | Enable registrar privacy for domain registry records; remove exposed documents, backup files, and administrative portals from public search engine indexes via `robots.txt` and search console removal tools. |
| **Infrastructure Mapping** *(Maltego, DNSrecon)* | **DNS Security Hardening** | Restrict DNS zone transfers (AXFR) to trusted secondary nameservers only; disable public directory listings and sanitize external-facing DNS records. |
| **Network & Port Scanning** *(Zenmap, Nmap)* | **Network Segmentation & Filtering** | Implement strict host-based and network firewall rules to block ICMP sweeps and unauthorized port probing; employ Intrusion Detection/Prevention Systems (IDS/IPS) to detect and rate-limit active network scans. |
| **Web Server Footprinting** *(WhatWeb, cURL, Wafw00f)* | **Banner Grabbing Defense & WAF Deployment** | Suppress or customize HTTP response headers and server tokens (e.g., `Server`, `X-Powered-By`); deploy a Web Application Firewall (WAF) with aggressive filtering rules. |

---
## 📍 Final Conclusion:

The execution of this network discovery and reconnaissance lab demonstrated the critical role that passive footprinting, open-source intelligence (OSINT), and active network scanning play in evaluating an organization's overall security posture. 

By leveraging tools such as **Whois**, **WhatWeb**, **NSlookup**, **theHarvester**, **GHDB**, and **Maltego**, an adversary can compile extensive intelligence regarding domain ownership, network infrastructure, web application frameworks, and personnel metadata—all without directly alerting target systems. Furthermore, active scanning via **Zenmap** on the target subnet (`192.168.56.0/24`) successfully mapped active host interfaces (`192.168.56.100`), illustrating how quickly open communication channels and network topologies can be identified.

Implementing the recommended countermeasures—including strict firewall access controls, server banner suppression, public data minimization, and hardened DNS configurations—significantly reduces the target attack surface and effectively mitigates the risk of unauthorized network exploitation.

---

## 🕸️ Encountered Problems and their Solutions:

* Problem 1:

Virtual Machine Network Communication Issue: 

Initially, the Kali Linux VM experienced network isolation, preventing it from establishing proper communication across the virtual environment. This occurred because the default virtual adapter settings restricted traffic routing. To resolve this, I navigated to VirtualBox Settings > Network, removed the non-functional adapter mode, and selected **NAT** mode to enable outbound network connectivity.

* Problem 2: 

Zenmap Visibility & Host Discovery Issue:

 I faced an issue where Zenmap and standard command prompt tools could not clearly display the IP address, MAC addresses, or determine whether target hosts were up or down—especially when connected to a mobile hotspot network. To resolve this, I switched to the Kali Linux terminal and executed the following commands to obtain full network visibility:

  1. **Identify Network Interface & IP Address:**
     ```bash
     ip a
     ```
     *Used to inspect active interfaces and verify the assigned local IP address and subnet.*

  2. **Discover Live Hosts & MAC Addresses:**
     ```bash
     sudo nmap -sn <ip address>
     ```
     *Executed a ping sweep with root privileges across the subnet to bypass discovery filters, accurately identify all live hosts, and retrieve their corresponding MAC addresses.*

---

## 🛠️ Resources: 

1. Kali Linux 

```bash
https://kali.org/get-kali
```

2. GHDB

```bash
https://www.exploit-db.com
```

3. Maltego

```bash
https://www.maltego.com/downloads/
```

4. Zenmap

```bash
https://nmap.org/zenmap/
```

---

## 👤 Author

NEHA

Cybersecurity Intern B083

LinkedIn: https://www.linkedin.com/in/neha-d-846342-nd

---

## 🎲 Project Information:

Program Name: Cybersecurity at Networkwalks | Week: 02 | Project: Cybersecurity-Footprinting and Reconnaissance | Repository: GitHub

---









