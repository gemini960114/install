# uv 安裝指南

## macOS

```bash
curl -LsSf https://astral.sh/uv/install.sh | sh
```

## Windows

```powershell
powershell -ExecutionPolicy ByPass -c "irm https://astral.sh/uv/install.ps1 | iex"
```

安裝是每個使用者各自安裝,不是系統全域,不需要系統管理員權限。

安裝位置:
- Windows: `%USERPROFILE%\.local\bin\uv.exe`
- macOS: `~/.local/bin/uv`

會自動寫入使用者層級 PATH,重開終端機即可直接用 `uv`。之後要查目前生效的位置:
- Windows(PowerShell):`(Get-Command uv).Source`
- macOS:`which uv`
