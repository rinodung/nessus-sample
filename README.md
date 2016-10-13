## Overview
Nessus® Home allows you to scan your personal home network (up to 16 IP addresses per scanner) with the same high-speed, in-depth assessments and agentless scanning convenience that Nessus subscribers enjoy.

Please note that Nessus Home does not provide access to support, allow you to perform compliance checks or content audits, or allow you to use the Nessus virtual appliance. If you require support and these additional features, please purchase a Nessus subscription.

Nessus Home is available for personal use in a home environment only. It is not for use by any commercial organization.

## Installation

1. Download Nessus from https://www.tenable.com/products/nessus/select-your-operating-system.
2. Choose the Ubuntu packages (or the Debian ones)
3. Open a Terminal and go to the download directory (cd)
4. Update Ubuntu: `sudo apt-get update` And Install dependency: `sudo apt-get -f install`
4. Run `sudo dpkg -i Nessus*.deb`. Enter root password.
5. Start it sudo /etc/init.d/nessusd start
6. Open a browser and go to https://localhost:8834/