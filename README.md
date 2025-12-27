[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)

# OWASP WAFControl Installer

The **OWASP WAFControl** project provides a web-based dashboard and management interface for ModSecurity and the OWASP Core Rule Set (CRS).  
It simplifies installation, configuration, and operation of CRS and ModSecurity, enabling administrators and security engineers to deploy, monitor, and manage WAF rules more effectively.


## Easy Install

```bash
curl -fsSL https://wafcontrol.org/download/install.sh -o install.sh
```

```bash
chmod +x install.sh
```

```bash
sudo ./install.sh
```
## Uninstall

WAFControl provides an interactive and safe uninstallation process.

⚠️ IMPORTANT

If Nginx or PostgreSQL were already installed on your server before WAFControl, DO NOT remove them.
Removing Nginx or PostgreSQL may break other applications and cause irreversible data loss.
If you remove them anyway, the responsibility is entirely yours.

The OWASP WAFControl project and its contributors are not responsible for data loss caused by manual or forced removal of system services.

```bash
curl -fsSL https://raw.githubusercontent.com/wafcontrol/install/refs/heads/main/uninstall.sh -o uninstall.sh
```

```bash
chmod +x uninstall.sh
```

```bash
sudo ./uninstall.sh
```


## WAFControl Resources
- [OWASP WAFControl Project Site](https://wafcontrol.org/)
- [OWASP WAFControl Project Page](https://owasp.org/www-project-wafcontrol/)  

## Documentation
- [OWASP WAFControl Docs](https://wafcontrol.org/docs)


## License

Copyright (c) 2025 OWASP WAFControl Project.  
All rights reserved.  

The OWASP WAFControl project is distributed under the Apache Software License (ASL) version 2.0.  
See the enclosed [LICENSE](./LICENSE) file for full details.