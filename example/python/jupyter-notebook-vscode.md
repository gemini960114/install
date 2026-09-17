幫我在 VS Code 裡設定一個能跑 Jupyter Notebook 的 Python 環境,用 uv 管理。整個專案建在 `D:\antigravity\game\jupyter-notebook-vscode`。

用 uv 建 venv,裝 `ipykernel` 就好(不用裝 `jupyterlab`,因為要用 VS Code 內建的 Jupyter 擴充套件開,不會用瀏覽器版介面)。建一份 `.ipynb`,寫一個 cell 印個東西測試就好。

在 VS Code 打開這份 `.ipynb`,右上角選 Kernel 時選 **Python Environments...**,選到這個 uv 建立的 venv(不要選 Existing Jupyter Server,那是連線到另外手動啟動的 Jupyter server 用的)。跑一下確認結果有正常顯示,就算設定成功。
