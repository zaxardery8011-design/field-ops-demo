# AGENTS.md — field-ops-demo

## 用途
單檔、手機優先的外勤打卡／派工／工作回報介面示範。事實來源是 `index.html`，不是正式工務後端。

## 目錄地圖
- `index.html`：HTML、CSS、JavaScript 與示範資料。
- `README.md`：最小使用方式；`LICENSE`：授權原文。

## 安裝與第一次執行
不需套件安裝或 build。用瀏覽器開啟 `index.html`。若電腦已有 Python，可在 repo 根目錄執行下列可選靜態伺服器，再開 http://localhost:8000/：
```bash
python -m http.server 8000 --bind 127.0.0.1
```
定位功能呼叫 `navigator.geolocation`，需要瀏覽器權限及可用定位環境；不保證直接開檔時每個瀏覽器都允許。

## 驗證
自動測試指令：未提供。人工檢查三個 tab、上下班打卡、新增派工、推進任務狀態、新增回報，重新整理後核對資料仍在。只用示範資料測。

## 不要做的事
資料在該瀏覽器的 localStorage（`wt_` 前綴），未提供伺服器同步、帳號驗證或多人權限管理。不要宣稱是正式考勤系統。`resetDemo()` 會呼叫 `localStorage.clear()`，不要在有其他同來源資料的環境隨意按重設。頁面名稱與預載人物／工地是現有示範內容，是否可公開真實資訊需由維護者確認。

## 同作者相關工具
- [task-ledger](https://github.com/zaxardery8011-design/task-ledger)：持久任務帳本，與本前端示範用途不同；本 repo 沒有接上它。
