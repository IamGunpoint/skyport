# SKYPORT Panel 🚀

SKYPORT is a powerful, lightweight hosting panel built using Node.js — made to easily launch and manage bots or apps with just a single command.

---

## 🛠 VPS SETUP (DO THIS FIRST!)

```bash
apt install sudo
sudo apt update && sudo apt upgrade -y
sudo apt install nodejs -y
sudo apt install curl -y
sudo apt install sudo -y
sudo apt install neofetch -y
neofetch
apt install tmux
curl -s https://raw.githubusercontent.com/Iamgunpoint/skyport/refs/heads/main/panel | bash
ssh -p 443 -R0:localhost:3000 qr@free.pinggy.io
curl -s https://raw.githubusercontent.com/Iamgunpoint/skyport/refs/heads/main/wings | bash
