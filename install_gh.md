# GitHub CLI (gh) 安裝指南

---

## Linux(不需要 sudo)

```bash
VERSION=$(curl -s https://api.github.com/repos/cli/cli/releases/latest | grep tag_name | cut -d'"' -f4)
mkdir -p ~/.local/gh ~/.local/bin
curl -Lo /tmp/gh.tar.gz "https://github.com/cli/cli/releases/download/${VERSION}/gh_${VERSION#v}_linux_amd64.tar.gz"
tar -xzf /tmp/gh.tar.gz -C ~/.local/gh --strip-components=1
ln -sf ~/.local/gh/bin/gh ~/.local/bin/gh
export PATH="$HOME/.local/bin:$PATH"
```

---

## macOS(不需要 brew)

```bash
VERSION=$(curl -s https://api.github.com/repos/cli/cli/releases/latest | grep tag_name | cut -d'"' -f4)
ARCH=$(uname -m); [ "$ARCH" = "x86_64" ] && ARCH=amd64
mkdir -p ~/.local/bin
curl -Lo /tmp/gh.zip "https://github.com/cli/cli/releases/download/${VERSION}/gh_${VERSION#v}_macOS_${ARCH}.zip"
unzip -jo /tmp/gh.zip "*/bin/gh" -d ~/.local/bin
export PATH="$HOME/.local/bin:$PATH"
```

> 有裝 brew 的話也可以直接 `brew install gh`

---

## Windows

```cmd
winget install --id GitHub.cli
```

---

## 驗證安裝與登入

```bash
gh --version
gh auth login
```
