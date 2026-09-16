# NETWORKWALKS-B083-WK2-CYBERSECURITY-FOOTPRINTING-Reconnaissance
Hands-on Cybersecurity lab using Kali Linux to practice Foot-printing and Reconnaissance.

# Footprinting in Cybersecurity 

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

































































  
