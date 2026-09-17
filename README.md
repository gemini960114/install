# install

常用開發工具的簡易安裝指南,涵蓋 Linux / macOS / Windows,每份文件只保留一行安裝指令加驗證方式。

## 文件列表

| 文件 | 說明 |
|---|---|
| [install_git.md](install_git.md) | Git 版本控制 |
| [install_gh.md](install_gh.md) | GitHub CLI(操作 GitHub 的命令列工具) |
| [install_nodejs.md](install_nodejs.md) | Node.js |
| [install_uv.md](install_uv.md) | uv(Python 套件與版本管理工具) |

## 建議教學順序

1. **Git**([install_git.md](install_git.md))— 版本控制基礎,其他步驟的前提
2. **GitHub CLI**([install_gh.md](install_gh.md))— 裝好後照 [example/setup/gh-auth.md](example/setup/gh-auth.md) 完成瀏覽器認證登入
3. **練習 commit/push**([example/setup/git-commit-push.md](example/setup/git-commit-push.md))— 學會存版本、推上 GitHub
4. **Node.js**([install_nodejs.md](install_nodejs.md))— 前端開發環境
5. **uv**([install_uv.md](install_uv.md))— Python 開發環境
6. **動手做範例**,由淺入深:
   - `example/html-js-canvas/` — 免建置,最快看到成果
   - `example/react/` — 練習 Node.js/React 工具鏈
   - `example/python/` — 練習 uv + 科學計算/生資工具
