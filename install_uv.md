# Astral `uv` 安裝指南

官方安裝腳本會自動把 `uv` 加入 PATH，重開終端機/重新登入也能直接用。

---

## Linux / macOS

```bash
curl -LsSf https://astral.sh/uv/install.sh | sh
```

> macOS 也可以用 Homebrew：`brew install uv`

---

## Windows

CMD 或 PowerShell 都可以：

```cmd
powershell -c "irm https://astral.sh/uv/install.ps1 | iex"
```

---

## 找不到指令怎麼辦

重新開一個終端機視窗再試一次（PATH 需要新視窗才會生效）。還是不行的話：

```bash
# Linux / macOS
export PATH="$HOME/.local/bin:$PATH"
```

```powershell
# Windows PowerShell
$env:PATH = "$HOME\.local\bin;$env:PATH"
```

---

## 常用指令

```bash
uv self update                          # 更新 uv
uv python install 3.12                  # 安裝 Python 版本
uv venv                                 # 建立虛擬環境
uv pip install requests pandas fastapi  # 安裝套件
```
