# Install Realtek r8168 driver on proxmox 8

1. Make sure `/etc/apt/sources.list` contains these lines:
```
deb http://ftp.nl.debian.org/debian bookworm main contrib non-free non-free-firmware
deb http://ftp.nl.debian.org/debian bookworm-updates main contrib non-free non-free-firmware
deb http://security.debian.org bookworm-security main contrib non-free non-free-firmware
deb http://download.proxmox.com/debian/pve bookworm pve-no-subscription
```
2. Install kernel headers: `apt install pve-headers`
3. Install r8168 driver: `apt install r8168-dkms`
4. Reboot

### Sources

https://forum.proxmox.com/threads/kernel-upgrade-and-pve-headers-installation.102093/  
https://forum.proxmox.com/threads/system-hanging-after-upgrade-nic-driver.129366/
