<img alt="gitleaks badge" src="https://img.shields.io/badge/protected%20by-gitleaks-blue">

# 🛡️ Micro-SaaS Security CI/CD Template

This repo provides a **plug-and-play GitHub Actions CI/CD pipeline** for micro-SaaS applications that want security scanning built in from day one.

## ✅ Features

- 🔍 Static Analysis via **Semgrep**
- 🧪 Dependency and Container Scanning via **Trivy**
- 🕷️ Dynamic Scanning via **OWASP ZAP**
- 🔐 Secret Detection via **Gitleaks**
- 📦 Dependency Updates via **Dependabot**
- 🧠 Optional CodeQL scans (free for public repos)

---

## 📦 Prerequisites

- GitHub repository (public or private)
- Basic CI/CD knowledge (GitHub Actions)
- Optional: Dockerfile, IaC files (for deeper Trivy scanning)

---

## 🚀 Quick Start

### 1. Fork this repo or copy the `.github/workflows/` folder into your project.

### 2. Create necessary configuration files:
- `semgrep.yml` (or use default ruleset)
- `trivy.yaml` (optional)
- `.gitleaks.toml` (optional custom config)

### 3. Add secrets (if needed)
Some tools may require tokens (e.g. `ZAP_AUTH`, `GITLEAKS_TOKEN`)

### 4. Watch it run! GitHub Actions will trigger on `push`, `PR`, or on a schedule.
