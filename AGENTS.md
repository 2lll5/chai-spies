# Agent Instructions

## Google Drive Build 交付規範（所有 Agent 必須遵守）
- Google Drive 位置：`AI Project/chai-spies/`（資料夾名稱與 GitHub Repo 完全相同；AI Project ID `1Yhfro6Ss5TSCXCVIZIHEu5h7V1gL8b27`）。禁止把 Build 散放於 `AI Project/` 根目錄。
- **最新且完整的版本直接放在專案資料夾根目錄**，包含 ZIP／EXE、SHA-256、完整分片與必要啟動／還原工具。不同平台最新版可以並存。上傳後讀回 Drive 的 parent、大小、名稱及校驗結果；缺 ZIP、checksum 或分片時不得取代上一完整版本。
- **只有功能／架構／相容性／重要美術差異，才建立 `vX.Y.Z-說明/` 版本子資料夾**。一般舊版非破壞性移到 `歷史封存/`，不得刪除。不要每次 Build 都新增版本資料夾。
- 只有完成實際 Build 與測試才可稱為已完成；所有開發提交 GitHub。昂貴 GitHub Actions 建置只在 `workflow_dispatch` 或正式 `release: published` 觸發，不隨每次 main push 執行。回報版本、Drive 專案目錄、檔案清單及校驗情況。

**Codex/agents (English):** Current complete builds go directly in `AI Project/chai-spies/`. Keep material milestones in version folders; archive ordinary older builds under `歷史封存/` without deletion; never promote incomplete uploads.
