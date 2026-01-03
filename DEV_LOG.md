開發時間紀錄（DEV_LOG）
專案資訊
*專案名稱：Kana Flashcards（日文假名學習卡）
*GitHub Repo：https://github.com/Alee3177/kana-flashcards
*GitHub Pages：https://alee3177.github.io/kana-flashcards/
*開發者：Anderson Lee / 李明隆
*公司：Opto Brilliant Ltd. 億立光股份有限公司
------------

開發總覽
 *開發起始日期：2025-12-29
 *最近一次更新：2026-01-03
 *主要開發天數：約 6 天
 *主要分支：
  -main：原始碼 / 邏輯開發
  -gh-pages：GitHub Pages 部署與 UI 調整
------------

Commit 統計（截至目前）
Branch	Commit 次數	用途
main	    12	    功能與原始碼開發
gh-pages	45	    網站部署、UI / RWD 修正
合計	        57	

備註：gh-pages commit 次數較多，原因是 UI/RWD 在手機與桌機間進行大量實測與微調。
------------

Branch：main（原始碼開發紀錄）
主要工作內容
*假名 Flashcard 核心架構
*卡片翻面（正面 / 背面）
*上一張 / 下一張 導覽
*行唸法 / 段唸法 / 行×段交錯出牌模式
*音效播放邏輯（翻面、點擊假名）
*選項控制：
 -加入濁音・半濁音
 -加入拗音
 -音效開關
 -移動後自動回正面
*.gitignore 設定與金鑰保護
*移除誤提交的 Google Cloud 金鑰（安全修復）

重點時間點
*2025-12-29：專案初始化、第一版可運行 Flashcard
*2025-12-30：出牌模式與音效邏輯完成
*2025-12-31：Git 歷史清理完成（安全）
------------

Branch：gh-pages（部署與 UI 調整紀錄）
主要工作內容
*GitHub Pages 發佈與維護
*聲音檔（sounds/）納入部署
*手機 / 桌機 RWD 調整
*Controls 區塊穩定化（2×2 checkbox）
*Button Row 改為 Grid（避免手機直立長柱）
*提示文字（提示 / 溫馨提醒）位置與視覺層級調整
*直式 / 橫式手機版實測修正

關鍵 UI 里程碑
*2026-01-02：
 -控制區在手機上維持左右排列
 -按鈕不再直立變柱

*2026-01-03：
 -「提示」與「溫馨提醒」顏色與層級定版
 -手機直式 / 橫式顯示位置正確
 -UI 結構最終穩定
------------

已確認穩定的 UI 區塊（⚠ 請勿任意修改）
以下區塊已反覆修正並確認穩定，未來如非必要請避免修改：
1..controls（2×2 Grid checkbox 區）
2..modeBlock / 出牌模式區結構
3..btnRow（Grid 版本，非 flex）
4.「提示」與「溫馨提醒」DOM 結構與顏色
5.音效觸發條件（避免自動誤播）
6..gitignore（金鑰與敏感檔案）
------------

風險紀錄與處理
問題	狀態	解法
金鑰誤提交	已解決	git filter-repo + .gitignore
手機 UI 崩壞	已解決	Grid-based layout
按鈕直立變柱	已解決	btnRow 改 Grid
提示位置跑版	已解決	結構固定 + media rules
------------

備註:
*本專案為「實際裝置導向」開發，所有 UI 決策皆以 真實手機（直式 / 橫式）實測 為依據。
*gh-pages commit 數量偏高屬正常現象，為 UI 微調與驗證所致。