---
layout: page
title: "Security Process"
desc: "Our security process ensures we keep customer data safe and aims to reduce the impact of a malicious attack"
permalink: /security/
---

**Local machine**

 * Your D4 email account must have a password of at least 16 characters and 2 factor authentication must be enabled.
 * 2 factor authentication is encouraged on other services, where it's available. E.g. github, stripe.
 * The company will provide an enterprise LastPass account for you, you should use this to generate and store secure 25+ character passwords for all online accounts and servers.
 * Sharing passwords around the team should be done by adding the passwords to a shared folder in LastPass, never via email or Slack.
 * Hard disk encryption should be turned on. This will ensure that if your device is lost, the data on that device is secure.


> Bonus points for using the [Firmware password](https://support.apple.com/en-gb/HT204455) on Mac which prevents the device from booting, even to another disk.


 * The company will supply an external hard drive for you, this should be used with your operating system's full-disk backup service (e.g. Time Machine on a Mac) to ensure you have a full disk backup and are not vunerable to a 'ransomware' attack.
   * You should plug in your backup disk regularly - the Mac will remind you periodically.
   * Your backup disk should also be encrypted to ensure that your data is secure if the backup disk is lost or stolen.
 * Project files should be stored in the appropriate Google Drive folder.
 * Your operating system should be configured to download and install security patches automatically.
 * Access to our systems/services given to clients should be logged in the Disclosure Log located on Google Drive. This should not include secure data such as passwords or certificates which should instead be stored in LastPass.
 * Access to clients systems/services should also be added to the Disclosure Log located on Google Drive. This should not include secure data such as passwords or certificates which should instead be stored in LastPass.
 * The Disclosure Log should be regularly reviewed and access revoked where no longer necessary.

**Code Repositories**

 * Production usernames, passwords, API keys, certificates and key files should never be checked into a repository. Store these as a secure note in LastPass instead.

**Servers**
 
 * Servers should be configured to download and install security patches automatically. E.g. on Ubuntu, install the 'unattended-upgrades' package:

```sh 
sudo apt-get install unattended-upgrades
```

```sh 
sudo dpkg-reconfigure unattended-upgrades
```

 * Servers should be hardened with a firewall (such as iptables) and services exposed through mature and well tested proxies (such as nginx).
 * Only essential services should be enabled and non-essential services turned off.
 * Root user should not be allowed SSH access. ```PermitRootLogin no```
 * Only allow SSH Protocol 2. ```Protocol 2```
 
