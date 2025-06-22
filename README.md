# PufferPanel 🚀

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
mkdir -p /var/lib/pufferpanel
docker volume create pufferpanel-config
docker create --name pufferpanel -p 8080:8080 -p 5657:5657 -v pufferpanel-config:/etc/pufferpanel -v /var/lib/pufferpanel:/var/lib/pufferpanel -v /var/run/docker.sock:/var/run/docker.sock --restart=on-failure pufferpanel/pufferpanel:latest
docker start pufferpanel
docker exec -it pufferpanel /pufferpanel/pufferpanel user add
ssh -p 443 -R0:localhost:8080 qr@free.pinggy.io
