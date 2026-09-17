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

前往 https://git-scm.com/download/win 下載安裝檔,直接執行安裝(一路 Next 即可)。

> 沒有系統管理員權限的話,下載同一頁面的 **Portable ("thumbdrive edition")** 版本,解壓到任意資料夾即可使用,不需要安裝。

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
