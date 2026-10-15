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

REST / GraphQL API security auditor (OpenAPI-driven)

---

## ✨ Features

- Own OpenAPI 2.0 (Swagger) / 3.0 / 3.1 JSON parser with local $ref resolution, servers / basePath, security schemes, parameters, request bodies and responses
- Plain endpoint-list loader ("GET /users/{id}" or URLs)
- Passive endpoint audit — missing auth, unsafe verbs, deprecated ops, rate-limit hints, verbose error schemas, sensitive params in query, mass-assignment hints, HTTP servers, weak auth schemes (basic / apiKey in query)
- Active checks (opt-in with --active, urllib, rate-limited): method tampering, missing-auth access, BOLA/IDOR hint, CORS misconfig, security headers, verbose errors, content-type confusion, enumeration / large response
- Auth tester — with vs without token comparison
- GraphQL — introspection detection, field-level hints
- Polite rate-limit probe (small burst → 429 expected)
- OWASP API Security Top 10 (2023) mapping, severity, remediation, risk score
- Export TXT / MD / JSON / CSV with location chooser
- Full CLI mode (--spec, --url, --active, --fail-on ...)

---

## ⚙️ Requirements

- **Linux**
- **No Python installation needed** — runs as a standalone executable

---

## 🚀 Usage

```bash
./OApiScan
```

---

## 📦 Part of OwlSec Toolkit

This tool is part of the **OwlSec** suite — a collection of 300+ security and privacy tools.

🔗 [owlsec.org](https://owlsec.org)

---

## ©️ License

MIT License — © Khaled S. Haddad

*Tools are distributed as pre-built executables. Source code is proprietary.*
