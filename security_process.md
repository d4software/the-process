---
layout: page
title: "Security Process"
desc: "Our security process ensures we keep customers data safe and that our operations are not interrupted by cyber attack"
permalink: /security/
---

 * Your D4 email account must have a password of at least 16 characters and 2 factor authentication must be enabled.
 * 2 Factor authentication is encouraged on other services, where it's available. E.g. github, stripe.
 * The company will purchase an enterprise LastPass account for you, you should use this to generate and store secure 25 character passwords for all online accounts and servers.
 * Sharing passwords around the team should be done by adding the passwords to a shared folder in LastPass, not via email or slack.
 * Hard disk encryption should be turned on. This will ensure that if your device is lost, the data on that device is secure.
 * The company will purchase an external hard drive for you, this should be used with your operating system's full disk backup service (e.g. Time Machine on a Mac) to ensure you have a full disk backup and are not vunerable to a ransomeware attack.
   * You should plug in your backup disk regularly.
   * Your backup disk should be encrypted to ensure that your data is secure if the backup disk is lost or stolen.
 * Project files should be stored in the appropriate Google Drive folder.
 * Your operating system should be configured to download and install security patches automatically.

**Code Repositories**

 * Production usernames, passwords, api keys, certificates and key files should never be checked into a repository. Store these as a secure note in LastPass instead.

**Servers**
 
 * Servers should be configured to download and install security patches automatically. E.g. on ubuntu, insall the 'unattended-upgrades' package:

    sudo apt-get install unattended-upgrades
    sudo dpkg-reconfigure unattended-upgrades

 * Servers should be hardened with a filewall (such as iptables) and servcies exposed through mature and well tested proxies (such as nginx)
