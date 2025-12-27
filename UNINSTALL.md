# WafControl – Uninstallation Guide

This document explains how to safely uninstall **WafControl** from your server.

> ⚠️ **Important**
>
> - This installer may have been run on servers that already had **Nginx** and/or **PostgreSQL** installed.
> - **By default, you should NOT remove Nginx or PostgreSQL** unless you are absolutely sure they were installed *only* for WafControl.
> - Removing system packages blindly can break other applications on the server.

---

## Uninstallation Options

You have **two supported ways** to uninstall WafControl:

1. **Interactive automatic uninstallation (recommended)**
2. **Manual uninstallation (advanced / fallback)**

---

## 1) Interactive Automatic Uninstallation (Recommended)

WafControl provides an **interactive uninstaller** that asks before removing each component.

### What this method does
- Stops and disables WafControl services
- Removes ModSecurity + CRS configuration
- Removes Nginx injections (load_module, WAF blocks)
- Optionally removes:
  - Application directory
  - PostgreSQL database and user
  - PostgreSQL packages
  - Nginx packages
- Uses recorded installer state when available
- **Asks for confirmation at every destructive step**

### How to run

```bash
sudo bash uninstall.sh
