# Docker 安裝指南

---

## Linux

```bash
curl -fsSL https://get.docker.com | sh
sudo usermod -aG docker $USER
```

> 執行完要重新登入(或 `newgrp docker`)才能不用 sudo 跑 docker。

---

## macOS

```bash
brew install --cask docker
```

> 裝完要手動開一次 Docker.app 才會啟動背景服務。

---

## Windows

> 需要先啟用 WSL2(沒開過的話先執行 `wsl --install`,重開機一次),否則 Docker Desktop 裝完會啟動失敗。

```cmd
winget install Docker.DockerDesktop
```

---

## 驗證安裝

```bash
docker --version
docker compose version
docker run hello-world
```
