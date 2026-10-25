# 🦉 OApiScan

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Linux-0a0c10?style=flat-square"/>
  <img src="https://img.shields.io/badge/Category-OWeb-blue?style=flat-square"/>
  <img src="https://img.shields.io/badge/License-MIT-green?style=flat-square"/>
  <img src="https://img.shields.io/badge/Part%20of-OwlSec%20Toolkit-7b5ea7?style=flat-square"/>
  <img src="https://img.shields.io/badge/Version-1.0.0-cyan?style=flat-square"/>
</p>

> **OApiScan** — REST / GraphQL API Security Auditor

---

> ⚠️ **AUTHORISED USE ONLY** — Use only on systems you own or have explicit written permission to test. Unauthorised use is illegal.

---

## 📌 Overview

OApiScan is a REST and GraphQL API security auditor that parses OpenAPI 2.0/3.x specifications (or plain endpoint lists) and runs a passive audit by default. With explicit authorisation it can enable benign active checks — method tampering, missing-auth access, BOLA/IDOR hints, CORS and security-header probes and a polite rate-limit burst. Findings are mapped to the OWASP API Security Top 10 (2023) with severity, remediation and a risk score.

---

## ✨ Features

- Built-in OpenAPI 2.0/3.0/3.1 parser with local $ref resolution
- Passive audit: missing auth, unsafe verbs, sensitive query params, weak schemes
- Opt-in active checks (--active): method tampering, BOLA/IDOR hints, CORS, headers
- Authentication tester comparing responses with and without a token
- GraphQL introspection detection and polite rate-limit probing
- OWASP API Top 10 (2023) mapping and export to TXT/MD/JSON/CSV

---

## ⚙️ Requirements

- **Linux**
- **No Python installation needed** — runs as a standalone executable

---

## 🚀 Usage

```bash
./OApiScan --spec openapi.json
./OApiScan --url https://api.example.com --active --token "Bearer xyz"
./OApiScan --graphql https://api.example.com/graphql --format json -o report.json
./OApiScan --help
```

---

## 📦 Part of OwlSec Toolkit

This tool is part of the **OwlSec** suite — a collection of 300+ security and privacy tools.

🔗 [owlsec.org](https://owlsec.org)

---

## ©️ License

MIT License — © Khaled S. Haddad

*Tools are distributed as pre-built executables. Source code is proprietary.*
