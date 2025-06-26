# Email Infrastructure DNS Hardening

This project sets up DNS records (SPF, DKIM, DMARC) to secure email delivery for a domain. It includes Cloudflare DNS automation with Terraform, testing tools, and sample configurations.
# 📧 Email Infrastructure DNS Hardening (SPF, DKIM, DMARC) using Terraform

This project automates the configuration of essential DNS records for email authentication using [Cloudflare DNS](https://www.cloudflare.com/dns/), managed through Terraform.

## 🚀 What it Does

- ✅ Adds **SPF** record for authorized mail servers  
- ✅ Adds **DKIM** record for cryptographic signing  
- ✅ Adds **DMARC** policy for reporting and security  

## 🧱 Tech Stack

- **Terraform** v1.5+
- **Cloudflare** DNS
- GitHub Actions (CI/CD)

## 📁 Files

- `main.tf` – DNS record definitions
- `.github/workflows/terraform.yml` – Terraform CI workflow

## 🔐 Requirements

- A [Cloudflare](https://dash.cloudflare.com) account
- Your domain must be managed via Cloudflare
- Cloudflare API Token with `Zone:DNS Edit` permission

## 🌍 How to Use

1. Clone this repo:
   ```bash
   git clone https://github.com/Kellykench/email-infrastructure-dns-hardening.git
   cd email-infrastructure-dns-hardening
