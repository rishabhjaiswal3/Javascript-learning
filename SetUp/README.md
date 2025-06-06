# 🧰 Development Environment Setup

This guide helps you install **Node.js**, **npm**, and **Visual Studio Code** on a Debian-based Linux system (like Ubuntu).

## 📦 Install VS Code

```bash
sudo apt update && sudo apt upgrade -y

sudo apt install software-properties-common apt-transport-https wget -y

wget -O- https://packages.microsoft.com/keys/microsoft.asc | sudo gpg --dearmor | sudo tee /usr/share/keyrings/vscode.gpg

echo "deb [arch=amd64 signed-by=/usr/share/keyrings/vscode.gpg] https://packages.microsoft.com/repos/vscode stable main" | sudo tee /etc/apt/sources.list.d/vscode.list

sudo apt update
sudo apt install code 
```


---

## 📦 Install Node.js & npm

```bash
sudo apt update
sudo apt upgrade

sudo apt install nodejs
sudo apt install npm

# Verify installation
node -v
npm -v
```