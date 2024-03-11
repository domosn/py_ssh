# 批次 SSH 連線和執行指令

這個 Python 程式使用到 `paramiko` 和 `openpyxl` 模組。

藉由讀取 Excel 檔案中的 SSH 設定，並批次連接到遠端伺服器執行指令。

## 安裝所需模組
```bash
pip install paramiko openpyxl
```

## 使用方法

1. 視實際情況，修改 file/setting.xlsx 檔案中的 username、password、hostname、port、command、execute、instructions 欄位內容(從第二列開始)。

    欄位說明:
    - command:使用(Alt+Enter)區隔每行指令
    - instructions:內容僅 y or yes(不分大小寫)會執行連線並執行

2. 執行 Python 程式。
    ```bash
    python ssh.py
    ```