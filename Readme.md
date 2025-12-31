![PowerShell](https://img.shields.io/badge/PowerShell-5.1+-blue.svg)
![Platform](https://img.shields.io/badge/Platform-Windows-lightgrey.svg)
# DNS Security Rotation Script

A PowerShell script that provides continuous DNS rotation between Cloudflare and Quad9 DNS servers for enhanced privacy and basic security hardening.

## Features
- Rotates DNS every 5 seconds in a 3-cycle pattern
- Enables Windows Firewall
- Disables high-risk services
- Clean shutdown with Ctrl+C
- Performance monitoring

## Usage
1. Run PowerShell as Administrator
2. Execute: `.\ContinuousDNSGuard.ps1`
3. Press Ctrl+C to stop

## Requirements
- Windows 10/11 with PowerShell 5.1+
- Administrator privileges

## Disclaimer
This script is for educational purposes. Use at your own risk.