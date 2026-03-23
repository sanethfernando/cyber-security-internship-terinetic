# Cyber Security Internship Treinetic

Prepared by: W. Saneth Fernando  
Target Application: DVWA (Damn Vulnerable Web Application)  
Testing Tools: Burp Suite Community Edition, Browser DevTools

---

## Overview

This repository contains the practical assessment submission for the Cyber Security Internship I made for Treinetic. The assessment involved setting up a vulnerable web application locally, identifying and exploiting five common web vulnerabilities, analysing the risks, and recommending fixes.

---

## Vulnerabilities Covered 

1. SQL Injection - Critical 
2. Cross-Site Scripting (XSS) - Medium 
3. Insecure Direct Object Reference (IDOR) - Medium 
4. Authentication Issues (Brute Force) - Critical 
5. Security Misconfiguration - Medium 


## Repository Structure

README.md - This file
report/ - Full security report in PDF format
screenshots/ - All evidence screenshots from testing

## Setup Instructions

### Prerequisites
- Docker Desktop installed and running
- Burp Suite Community Edition

### Running DVWA

1. Open terminal and run:

"docker run --rm -it -p 80:80 vulnerables/web-dvwa"

2. Open browser and go to `http://localhost/setup.php`

3. Click **Create / Reset Database**

4. Go to `http://localhost/login.php` and login:
   - Username: `admin`
   - Password: `password`

5. Go to **DVWA Security** → set level to **Low** → click Submit

### Setting Up Burp Suite

1. Open Burp Suite → Temporary project → Start Burp
2. Click **Proxy** tab → **Open Browser**
3. Use the Burp browser for all testing to route traffic through the proxy


## Full Report

The complete security report including all findings, risk analysis, and mitigation recommendations is available in the `/report` folder.
