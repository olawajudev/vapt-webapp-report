# 📄 Web Application Pentest Report (Sanitized Sample)
> Professional VAPT engagement deliverable – Lab Environment Only

![Status](https://img.shields.io/badge/Status-Sanitized%20Sample-blue)
![Methodology](https://img.shields.io/badge/Methodology-OWASP%20PTES-green)
![License](https://img.shields.io/badge/License-CC--BY--NC--4.0-lightgrey)

This repository contains a **sanitized, educational sample** of a web application penetration test report. All findings, IPs, and identifiers are fictional and derived from authorized lab testing (OWASP Juice Shop, Metasploitable).

> ⚠️ **Disclaimer**: This report is for portfolio/educational demonstration only. No real systems were tested. All vulnerabilities are documented in isolated lab environments with explicit authorization.

---

## 📋 Report Contents
| File | Description |
|------|-------------|
| [`reports/webapp-pentest-sample.md`](reports/webapp-pentest-sample.md) | Full Markdown report (7 findings, CVSS v3.1, PoC, remediation) |
| [`reports/executive-summary.pdf`](reports/executive-summary.pdf) | 1-page executive summary (PDF) |
| `docs/methodology.md` | Testing methodology, scope, tools used |
| `docs/ethics.md` | Ethics framework, lab setup, authorization notes |

---

## 🔍 Sample Findings Overview
| ID | Vulnerability | Location | CVSS | Severity |
|----|---------------|----------|------|----------|
| WEB-001 | SQL Injection (Login) | `/login` | 9.8 | Critical |
| WEB-002 | IDOR (User Profile) | `/api/user/{id}` | 7.5 | High |
| WEB-003 | Weak JWT Secret | Auth Module | 8.1 | High |
| WEB-004 | Reflected XSS | Search Param | 6.1 | Medium |
| WEB-005 | Missing Security Headers | Global | 4.3 | Medium |
| WEB-006 | Verbose Error Messages | API Endpoints | 3.7 | Low |
| WEB-007 | Outdated Library (jQuery) | Frontend | 5.3 | Medium |

---

## 🧪 Lab Environment Details
- **Target Application**: OWASP Juice Shop v15.0.0 (Docker)
- **Network**: Isolated VirtualBox NAT (`192.168.56.0/24`)
- **Tools Used**: Burp Suite Community, Nmap, SQLmap (lab mode), custom Python scripts
- **Testing Window**: 4 hours (authorized scope only)

---

## 📬 Contact
For questions about this sample report or methodology:
- GitHub: [@olawajudev](https://github.com/olawajudev)
- LinkedIn: https://linkedin.com/in/olanrewaju-ayo
- TryHackMe: [wajudev](https://tryhackme.com/p/wajudev)
