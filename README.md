# field-ops-demo

給想看外勤介面流程的人使用的單檔示範：上下班打卡、工地派工與工作回報。HTML、CSS、JavaScript 都在 `index.html`；不需要套件安裝或 build。頁面資料皆為虛構示範。

## 第一次使用
下載或 clone 本 repo，以瀏覽器開啟 `index.html`。若已有 Python，也可在此資料夾執行：
```bash
python -m http.server 8000 --bind 127.0.0.1
```
再開 http://localhost:8000/ 。用示範資料試三個 tab、新增派工與新增回報。定位需要瀏覽器允許；能否取得位置取決於環境。

## 範圍與限制
資料留在同一瀏覽器的 localStorage，重新整理會讀回；沒有後端、帳號驗證或多人同步。頁面內有預載示範資料。不是正式考勤、薪資或派工管理系統。重設示範會清空該來源的 localStorage，請用專用來源測試。

自動測試指令：未提供。AI 助理先讀 [AGENTS.md](AGENTS.md)，實作以 [index.html](index.html) 為準。授權見 [LICENSE](LICENSE)。

## 同作者相關工具
- [task-ledger](https://github.com/zaxardery8011-design/task-ledger)：單機持久任務帳本；沒有與本示範接線。
