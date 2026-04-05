# 🕸️ ODirHunt

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Linux%20%2F%20Windows-informational?style=flat-square&logo=linux&logoColor=white&color=0a0c10"/>
  <img src="https://img.shields.io/badge/Category-ORec%20%2F%20Web%20Recon-cyan?style=flat-square"/>
  <img src="https://img.shields.io/badge/Dependencies-requests%20beautifulsoup4-yellow?style=flat-square"/>
  <img src="https://img.shields.io/badge/License-Proprietary-green?style=flat-square"/>
  <img src="https://img.shields.io/badge/Part%20of-OwlSec%20Toolkit-7b5ea7?style=flat-square"/>
  <img src="https://img.shields.io/badge/Version-v2.0-cyan?style=flat-square"/>
</p>

> **ODirHunt** is a powerful multi-threaded web crawler and inventory discovery suite. It discovers endpoints, parses sitemap.xml and robots.txt, fingerprints headers, detects forms, extracts links, and exports findings to JSONL, CSV, and TXT.

**Perfect for web reconnaissance, attack surface mapping, and authorized security testing.**

---

## 📌 Overview

ODirHunt crawls websites intelligently while respecting robots.txt (optional), discovering sitemaps, following links within depth limits, and collecting rich metadata (status codes, content types, titles, security headers, technologies, forms, etc.).

It supports quick scans for speed and full deep crawls for thoroughness, with configurable filters and rate limiting.

---

## 🖥️ Modules

| # | Module                  | Description |
|---|-------------------------|-------------|
| **[1]** | **Quick Crawl**         | Fast scan (depth=1, limited pages) |
| **[2]** | **Full Crawl**          | Deep scan with all features enabled |
| **[3]** | **Sitemap Scan**        | Parse sitemap.xml and crawl discovered URLs |
| **[4]** | **Robots Inspect**      | Fetch and display robots.txt content |
| **[5]** | **Last Report**         | View summary of the last crawl |
| **[6]** | **Export**              | Save findings as JSON |
| **[7]** | **Settings**            | Configure target, threads, depth, filters, output |

---

## 📊 Key Features

- **Multi-threaded Crawling** — Configurable threads and depth
- **Sitemap & Robots Support** — Automatic discovery and respect (optional)
- **Rich Fingerprinting** — Security headers (HSTS, CSP, X-Frame, etc.), technologies, forms
- **Form Detection** — Login, search, upload, register forms
- **Filtering** — By status codes, content types, size, title keywords
- **Rate Limiting** — Delay + jitter to avoid detection
- **Multiple Export Formats** — JSONL (structured), CSV, TXT
- **Clean Terminal UI** — Colored output with progress and summary

---

## ⚙️ Requirements

- **requests**
- **beautifulsoup4**
  ```bash
  pip install requests beautifulsoup4
  chmod +x ODirHunt
  ./ODirHunt

  📁 Output

Live Terminal — Real-time colored results with status, title, tech, and forms
Reports (in odirhunt_results/):
odirhunt_<target>_<timestamp>.jsonl — Full structured findings
odirhunt_<target>_<timestamp>.csv — Spreadsheet format
odirhunt_<target>_<timestamp>.txt — Plain URL list with metadata



📦 Part of OwlSec Toolkit
This tool is part of the OwlSec suite — a collection of 300+ security and privacy tools.
🔗 owlsec.org

©️ License
Proprietary — © Khaled S. Haddad
Tools are distributed as pre-built executables. Source code is proprietary.
AUTHORISED WEB RECONNAISSANCE & SECURITY TESTING USE ONLY
