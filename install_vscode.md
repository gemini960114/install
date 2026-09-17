# VS Code 安裝指南

---

## Linux

```bash
# Debian / Ubuntu
sudo apt-get update && sudo apt-get install -y wget gpg
wget -qO- https://packages.microsoft.com/keys/microsoft.asc | gpg --dearmor > packages.microsoft.gpg
sudo install -D -o root -g root -m 644 packages.microsoft.gpg /etc/apt/keyrings/packages.microsoft.gpg
echo "deb [arch=amd64,arm64,armhf signed-by=/etc/apt/keyrings/packages.microsoft.gpg] https://packages.microsoft.com/repos/code stable main" | sudo tee /etc/apt/sources.list.d/vscode.list
sudo apt-get update && sudo apt-get install -y code
```

---

## macOS

```bash
brew install --cask visual-studio-code
```

---

## Windows

```cmd
winget install --id Microsoft.VisualStudioCode -e
```

---

## 驗證安裝

```bash
code --version
```
