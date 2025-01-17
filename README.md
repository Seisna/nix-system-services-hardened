# nix-system-services-hardened

<h3 align="left">
  <div>
    <a href="https://github.com/YvesCousteau/nix-system-services-hardened/issues">
        <img src="https://img.shields.io/github/issues/YvesCousteau/nix-system-services-hardened?color=cc241d&labelColor=fbf1c7&style=for-the-badge">
    </a>
    <br>
    <a href="https://github.com/YvesCousteau/nix-system-services-hardened/stargazers">
        <img src="https://img.shields.io/github/stars/YvesCousteau/nix-system-services-hardened?color=98971a&labelColor=fbf1c7&style=for-the-badge">
    </a>
    <br>
    <a href="https://github.com/YvesCousteau/nix-system-services-hardened/">
        <img src="https://img.shields.io/github/repo-size/YvesCousteau/nix-system-services-hardened?color=d79921&labelColor=fbf1c7&style=for-the-badge">
    </a>
    <br>
    <img src="https://img.shields.io/badge/NixOS-25.05.20250113.9abb87b (Warbler)-blue?color=blue&labelColor=fbf1c7&style=for-the-badge">
    <br>
  </div>
</h3>

## :zap: Hardening Result

System services hardened (lynis BOOT-5264) under nixos.\
Suggest you to see https://linux-audit.com, if you are interested of how to hardened your config.

```sh
❯ systemd-analyze security
UNIT                                  EXPOSURE PREDICATE HAPPY
--------------------------------------------------------------
NetworkManager-dispatcher.service          3.5 OK        🙂
NetworkManager.service                     4.2 OK        🙂
accounts-daemon.service                    2.9 OK        🙂
acpid.service                              4.8 OK        🙂
auditd.service                             4.0 OK        🙂
blocky.service                             4.2 OK        🙂
bluetooth.service                          4.7 OK        🙂
colord.service                             4.9 OK        🙂
cups.service                               4.8 OK        🙂
dbus.service                               4.2 OK        🙂
display-manager.service                    4.8 OK        🙂
docker.service                             4.8 OK        🙂
getty@tty1.service                         4.7 OK        🙂
getty@tty2.service                         4.7 OK        🙂
getty@tty7.service                         4.7 OK        🙂
nix-daemon.service                         4.9 OK        🙂
nscd.service                               4.9 OK        🙂
polkit.service                             1.2 OK        🙂
reload-systemd-vconsole-setup.service      4.9 OK        🙂
rescue.service                             4.5 OK        🙂
rtkit-daemon.service                       3.1 OK        🙂
sshd.service                               4.9 OK        🙂
systemd-ask-password-console.service       4.3 OK        🙂
systemd-ask-password-wall.service          4.1 OK        🙂
systemd-hostnamed.service                  1.7 OK        🙂
systemd-journald.service                   4.5 OK        🙂
systemd-logind.service                     2.8 OK        🙂
systemd-machined.service                   3.0 OK        🙂
systemd-oomd.service                       1.8 OK        🙂
systemd-rfkill.service                     4.0 OK        🙂
systemd-timesyncd.service                  2.1 OK        🙂
systemd-udevd.service                      4.9 OK        🙂
user@1000.service                          4.8 OK        🙂
wpa_supplicant.service                     2.7 OK        🙂
```

## ⌨️ Commands

* Check service log: `journalctl -u SERVICE_NAME`
* Check service security: `systemd-analyze security SERVICE_NAME`
* Check services security: `systemd-analyze security`

## :book: Note
1. Why i did it:
    * I didn't find any repo which provide hardened system service configs.
    * So the idea merged i my head to do it for nix lovers and others.
2. What you can find inside this repo:
    * Each system service config file for listed above.
3. Keep in mind:
    * I know it's not perfect, i want to give you help that i couldn't find.
    * If you want to suggest any improvement, make a PR. 
    * If you find any error, make an issue. 

## 📜 License

Apache License - see the [LICENSE](LICENSE) file for details.

## 💝 Acknowledgements

Love u guys 💜.\
Buy me a coffe if you've a mind to:`1CJwob8qgoX7e897fupbyu3VbATMkgBpwM`\
\
![image](./qr-btc.png)
