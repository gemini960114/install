# Git 安裝指南

---

## Linux

```bash
# Debian / Ubuntu
sudo apt-get update && sudo apt-get install -y git

# CentOS / RHEL / Fedora
sudo yum install -y git
```

---

## macOS

```bash
brew install git
```

> 沒有 Homebrew 也可以直接執行 `git --version`，macOS 會跳出提示安裝 Xcode Command Line Tools。

---

## Windows

```cmd
winget install --id Git.Git -e --source winget
```

---

## 驗證安裝

```bash
git --version
```

---

## 常用設定

```bash
git config --global user.name "你的名字"
git config --global user.email "you@example.com"
```
