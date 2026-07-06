# GitHub 中文化插件（正體單檔維護版）

這是一個用於將 GitHub 網頁介面翻譯為**正體中文**的 Userscript（使用者腳本），旨在為習慣正體中文的使用者提供更易讀的 GitHub 瀏覽體驗。

## 📌 專案由來與致謝 (Credits & Origin)

本專案是基於開源社群前輩的心血修改而來，並遵守 **GPL-3.0 開源協議**：
- **原始專案**：[github-chinese](https://github.com/maboloshi/github-chinese)
- **原創作者**：[樓教主 (52cik)](https://github.com/52cik)
- **後續主要維護者**：[沙漠之子 (maboloshi)](https://github.com/maboloshi)

## 🚀 本版本特色與改進 (Features)

在原專案的基礎上進行了以下調整與優化：

1. **單檔案架構 (Single File Integration)**
   將原本分離的控制腳本與詞庫（`locals.js`）合併為單一 `JSON / Userscript` 檔案，徹底解決外部依賴與安裝繁瑣的問題，簡化更新流程。
3. **支援 GitHub 最新功能 (Modern GitHub UI Support)**
   本專案新增了對 GitHub 最新介面與動態加載組件的中文化支持，包括但不限於：
   - GitHub Copilot 對話框與 AI 代理頁面
   - GitHub Spark
   - MCP Registry (Model Context Protocol) 及其詳情頁面
   - 新版全域搜尋結果、主題探索 (Topics)、贊助頁面 (Sponsors)
4. **修復動態載入的英文殘留 Bug (Dynamic DOM Fixes)**
   實作了更密集的重試機制與精確的 DOM 攔截，有效解決了 GitHub 使用 React、Turbo 與 Shadow DOM 渲染時，刷新頁面後中文又變回英文的閃爍與殘留問題。

## 🛠️ 安裝方式

1. 首先安裝使用者腳本管理器，例如：[Tampermonkey](https://www.tampermonkey.net/) 或 [Violentmonkey](https://violentmonkey.github.io/)；
2. 將下載的 GitHub-TransCHT-Userscript.json 新增到油猴中並啟用；
3. 重新整理你的 GitHub 頁面即可生效。

## 📄 授權協議 (License)

本專案沿用原始專案的 [GPL-3.0 License](https://www.gnu.org/licenses/gpl-3.0.html)。
你可以自由地使用、修改及散佈本程式碼，但請務必遵守該協議保留原作者與本專案的版權聲明，並且任何衍生作品也必須以 GPL-3.0 開源發佈。
