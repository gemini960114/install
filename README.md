# vscode-dev-onboarding

給學生的本地端開發環境教學材料:用 VS Code 在 Linux / macOS / Windows 安裝常用開發工具,再透過一系列動手做範例練習上手。

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
     - [four-bar-linkage.md](example/html-js-canvas/four-bar-linkage.md) — 曲柄搖桿機構動畫
     - [snake.md](example/html-js-canvas/snake.md) — 貪食蛇遊戲
   - `example/react/` — 練習 Node.js/React 工具鏈
     - [four-bar-linkage-react.md](example/react/four-bar-linkage-react.md) — 曲柄搖桿機構動畫(React 版)
     - [snake-react.md](example/react/snake-react.md) — 貪食蛇遊戲(React 版)
   - `example/python/` — 練習 uv + 科學計算/生資工具
     - [health-data-analysis.md](example/python/health-data-analysis.md) — 登革熱病例資料分析(requests + pandas + matplotlib)
     - [multiqc-report.md](example/python/multiqc-report.md) — MultiQC 定序 QC 報告彙整
     - [jupyter-notebook-vscode.md](example/python/jupyter-notebook-vscode.md) — 在 VS Code 用 uv 設定可跑 Jupyter Notebook 的 Python 環境
     - [multiqc-report-notebook.md](example/python/multiqc-report-notebook.md) — 延續 multiqc-report,補上 Jupyter Notebook 互動式分析
     - [health-data-analysis-notebook.md](example/python/health-data-analysis-notebook.md) — 延續 health-data-analysis,補上 Jupyter Notebook 互動式分析
