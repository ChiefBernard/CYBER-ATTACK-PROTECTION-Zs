# 🔄 Continuous DNS Security Rotator

A robust PowerShell script that continuously rotates DNS servers between Cloudflare (1.1.1.1) and Quad9 (9.9.9.9) to enhance privacy and provide basic security hardening.

![PowerShell Version](https://img.shields.io/badge/PowerShell-5.1+-blue.svg)
![Platform](https://img.shields.io/badge/Platform-Windows-lightgrey.svg)
![License](https://img.shields.io/badge/License-MIT-green.svg)

## ✨ Features

- **Continuous DNS Rotation**: Automatically switches between Cloudflare and Quad9 DNS every 5 seconds
- **Security Hardening**: Enables Windows Firewall and disables high-risk services
- **Clean Operation**: Graceful shutdown with Ctrl+C that restores original DNS settings
- **Visual Feedback**: Real-time console display with rotation statistics
- **Persistent State**: Maintains rotation cycle across restarts

## 🚀 Quick Start

### Prerequisites
- Windows 10/11
- PowerShell 5.1 or higher
- **Administrator privileges**

### Installation
```powershell
# Clone the repository
git clone https://github.com/YOUR-USERNAME/DNS-Security-Rotation.git
cd DNS-Security-Rotation

# Run the script (as Administrator)
.\ContinuousDNSGuard.ps1
```

## 📋 Usage

```powershell
# Start the DNS rotation service
.\ContinuousDNSGuard.ps1

# Press Ctrl+C to stop and restore original DNS settings
```

**Expected Output:**
```
[14:30:25] ✓ ☁️ Cloudflare   State: CF1 Rotations: 1 (12.00/min)
[14:30:30] ✓ 🛡️ Quad9        State: Q9  Rotations: 2 (24.00/min)
```

## ⚙️ Configuration

Edit the script to modify:
- Rotation interval (`$RotationDelay`)
- DNS servers (`$CloudflareDNS`, `$Quad9DNS`)
- Services to disable (in `Initialize-SecurityBaseline`)

## ⚠️ Disclaimer

This tool is for **educational and privacy-enhancement purposes** only. Use at your own risk. The authors are not responsible for any network disruptions or security issues caused by this software.

## 📄 License

Distributed under the MIT License. See `LICENSE` for more information.

## ☕ Support This Project

If this tool helps protect your privacy and you'd like to support its development:

[![Stripe](https://img.shields.io/badge/Donate-Stripe-635bff)](https://buy.stripe.com/dRm5kDch65VN2vJcrKgw005)
[![GitHub Sponsors](https://img.shields.io/badge/Sponsor-GitHub-%23EA4AAA)](https://github.com/sponsors/ChiefBernard)

Your support helps cover:
- Server costs for testing
- Development time for new features
- Security audits and updates