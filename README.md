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
5. Start it `sudo /etc/init.d/nessusd start`
6. Open a browser and go to https://localhost:8834/
7. 

## Usage
1. View the Current Network Interfaces
 `/opt/nessus/sbin/nessuscli fix --list-interfaces1`
2. Resetting Registration and Erase SettingsTo reset the registration information,
 shut down the nessusdservice first. 
 Next, run the nessuscli fix --resetcommand. 
 You will be prompted for confirmation.
 If you have not shut down the nessusdservice, 
 the nessuscli fix --resetcommand will exit.
3. Change default port
` /opt/nessus/sbin/nessuscli fix --set xmlrpc_listen_port=80`
4. List all interfaces
`/opt/nessus/sbin/nessuscli fix --list-interfaces`


```
 # /sbin/service nessusd stop
 # /opt/nessus/sbin/nessuscli fix --resetResetting Nessus configuration will permanently erase all your settings and cause Nessus to become unregistered.
Do you want to proceed? (y/n) [n]: y
Successfully reset Nessus configuration
```