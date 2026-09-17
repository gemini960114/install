延續 `multiqc-report.md` 那個專案(`D:\antigravity\multiqc-report`),現在要在同一個 venv 裡加開 Jupyter Notebook,對 MultiQC 產生的資料做第二輪分析,不只是看那份彙整好的 HTML 報告。

用 `uv pip install ipykernel pandas nbformat` 補裝進同一個 venv 就好(不用重建 venv,MultiQC 本來裝的套件保留)。裝 `pandas` 是因為要讀取 MultiQC 匯出的表格資料,裝 `nbformat` 是因為 `plotly` 的圖要在 notebook 裡用 `fig.show()` 顯示,沒裝會噴 `Mime type rendering requires nbformat>=4.2.0` 的錯誤。

MultiQC 產生報告時,除了那份 HTML,還會在報告資料夾旁邊留一個 `_data` 資料夾(裡面一堆 `.txt`,其實是 tab 分隔的表格,像 `multiqc_general_stats.txt`、`samtools-flagstat-table.txt`、`multiqc_fastqc.txt` 這種)。寫一份 `.ipynb`,用 `pandas` 把這些檔案讀進來,整理成表格,再挑幾個指標畫圖看看,例如:

- 各樣本的 mapped reads 或 coverage 長條圖
- FastQC 的 %GC 分布直方圖
- coverage 對 mean depth 的散佈圖

在 VS Code 打開這份 `.ipynb`,右上角選 Kernel 時選 **Python Environments...**,選到這個專案的 uv venv,跑一下確認圖表有正常顯示。
