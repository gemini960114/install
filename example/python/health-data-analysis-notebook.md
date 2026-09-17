延續 `health-data-analysis.md` 那個專案(`D:\antigravity\game\health-data-analysis`),現在要在同一個 venv 裡加開 Jupyter Notebook,把 `analyze_dengue.py` 的分析邏輯搬進 notebook 互動式重現,並多做幾個延伸分析。

用 `uv pip install ipykernel` 補裝進同一個 venv 就好(`pandas`、`matplotlib`、`requests` 原本就裝著了,不用重裝,也不用重建 venv)。資料沿用腳本已經快取好的 `data/dengue_daily.csv`,不用重新下載。

寫一份 `.ipynb`,拆成幾個 cell:

- 讀取、前處理資料(跟 `analyze_dengue.py` 的 `load_and_preprocess()` 邏輯一致)
- 重現原本腳本的兩張圖,但直接用 `plt.show()` 顯示在 notebook 裡,不要只存成 PNG:
  - 各縣市病例數排名長條圖
  - 病例數最高縣市的逐月趨勢折線圖
- 延伸分析,至少加這幾個原本腳本沒畫的角度:
  - 全台歷年病例數趨勢(先看長期趨勢,再說明為什麼挑這一年出來細看)
  - 性別、年齡層分布
  - 本土病例 vs 境外移入病例的比例

每個分析區塊前面都要寫詳細的中文說明,包含這個指標代表什麼、看到什麼樣的結果算正常或異常,不要只有程式碼。

在 VS Code 打開這份 `.ipynb`,右上角選 Kernel 時選 **Python Environments...**,選到這個專案的 uv venv,Run All 確認所有圖表都能正常顯示。
