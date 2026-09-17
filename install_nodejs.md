# Node.js 安裝指南

---

## Linux / macOS

推薦用 nvm 安裝，方便切換版本：

```bash
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.40.1/install.sh | bash
```

安裝完重開終端機，再安裝 Node.js：

```bash
nvm install --lts
```

> macOS 也可以直接用 Homebrew：`brew install node`

---

## Windows

```cmd
winget install OpenJS.NodeJS.LTS
```

---

## 驗證安裝

```bash
node --version
npm --version
```
