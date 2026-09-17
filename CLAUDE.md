# 專案規則

- 這個專案需要用 Python 時,一律用 `uv` 管理環境與執行,不要直接呼叫系統原生的 `python`/`pip`。
  - 建立環境:`uv venv`
  - 安裝套件:`uv pip install <package>`
  - 執行程式:`uv run <script>.py`
