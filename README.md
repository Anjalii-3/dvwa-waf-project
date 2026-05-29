# DVWA + WAF Security Lab

## 📌 Project Overview

This project demonstrates how a vulnerable web application can be attacked using SQL Injection and how a Web Application Firewall (WAF) can be used to prevent such attacks.

## 🧱 Technologies Used

* Docker
* Nginx (as WAF)
* DVWA (Damn Vulnerable Web Application)
* Linux (WSL)

## ⚙️ Setup Instructions

1. Clone the repository:
   git clone https://github.com/Anjalii-3/dvwa-waf-project.git

2. Navigate to the project:
   cd dvwa-waf-project

3. Start the containers:
   sudo docker compose up -d

4. Open browser:
   http://localhost:8080

---

## 💣 Attack Demonstration (SQL Injection)

Input:
1' OR '1'='1

Result:

* Without WAF → All user data is displayed (vulnerability exploited)

---

## 🛡️ WAF Protection

Nginx is configured to detect and block SQL injection patterns.

Blocked patterns include:

* '
* OR

---

* #

Result:

* With WAF → Attack is blocked (403 Forbidden)

---

## 🧠 Key Learnings

* Understanding SQL Injection attacks
* How web applications interact with databases
* Importance of input validation
* Role of Web Application Firewalls (WAF)
* Using Docker for environment setup

---

## 🚀 Project Outcome

Successfully demonstrated:

* Vulnerability exploitation
* Implementation of security defense
* Real-world cybersecurity workflow

