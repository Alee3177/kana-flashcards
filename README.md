\# 日語50音平假名-片假名對應閃卡練習(kana-flashcards); 初學者學習工具

一款專為日語初學者打造的手機優先學習工具，讓學習更簡單、更直覺、更容易開始。

A mobile-first learning tool designed to make Japanese learning easy and accessible for beginners.

---


\## 開發設計者｜Developer
\- Anderson Lee / 李明隆  
\- Opto Brilliant Ltd. 億立光股份有限公司

---


\## 開發宗旨｜Project Purpose

本專案的開發宗旨，是為了讓每一位日語初學者，都能擁有一個\*\*簡單、直覺、好上手的學習工具\*\*。  
整體設計特別針對「手機端直接使用」的情境進行最佳化，讓學習不再受限於時間、地點或設備，隨時隨地都能開始練習。

本工具著重於\*\*操作流程最小化與介面清楚化\*\*，即使不閱讀說明文件，使用者也能立即上手，  
將學習重心放在語言本身，而非工具操作。

---

The purpose of this project is to provide a \*\*simple, intuitive, and easy-to-use tool\*\* for Japanese language beginners.  
It is designed with a \*\*mobile-first approach\*\*, enabling learners to study anytime and anywhere.

The tool focuses on \*\*minimal interaction steps and a clean interface\*\*, allowing users to start learning immediately without reading extensive documentation.

---


\## 適合對象｜Target Users

\- 日語初學者  
\- 希望利用零碎時間進行學習的使用者  
\- 以手機為主要學習裝置的學習者  
\- 重視操作簡單、能快速開始的學習者  

---

\- Japanese language beginners  
\- Learners who study in short, flexible sessions  
\- Mobile-first learners  
\- Users looking for an out-of-the-box learning experience  


---

\## 功能特色｜Features

\### 📱 手機優先設計（Mobile-First）

\- 介面與操作流程以手機使用情境為核心設計  
\- 無需複雜設定，打開即可使用，適合隨時隨地學習  

Designed with a mobile-first approach, optimized for smartphones.  
No complex setup required—users can start learning immediately, anytime and anywhere.

---


\### 🔤 平假名／片假名學習支援

\- 支援平假名與片假名的基礎學習與辨識  
\- 適合初學者建立日文文字基礎  

Supports basic learning and recognition of Hiragana and Katakana,  
helping beginners build a solid foundation in Japanese writing systems.

---


\### 🔊 發音輔助（Audio Support）

\- 提供日文發音輔助，協助建立正確語感  
\- 適合搭配視覺記憶與反覆練習使用  

Provides audio pronunciation support to help learners develop accurate listening and speaking intuition.  
Ideal for repeated practice combined with visual memorization.

---


\### 🧩 操作流程極簡化

\- 學習流程經過簡化，降低操作負擔  
\- 不需閱讀說明文件，也能直覺使用  

The learning flow is intentionally simplified to reduce operational overhead.  
Users can interact intuitively without reading extensive documentation.

---


\### 🎯 專注初學者需求

\- 功能設計聚焦於「入門階段真正需要的內容」  
\- 避免過多進階設定，降低學習壓力  

Features are carefully scoped to match the real needs of beginners,  
avoiding unnecessary complexity and reducing learning friction.

---


\### 🔄 適合碎片化學習

\- 每次使用時間彈性，適合短時間反覆練習  
\- 有助於培養穩定、長期的學習習慣  

Designed for short, flexible learning sessions,  

supporting consistent practice and long-term learning habits.

---


\## 專案精神｜Project Vision

本專案希望\*\*降低日語學習的入門門檻\*\*，讓更多人能以輕鬆、可持續的方式接觸並累積日語能力，  
並透過簡單而有效的工具設計，培養長期學習的習慣。

This project aims to lower the barrier to learning Japanese and encourage sustainable, long-term learning through thoughtful and simple tool design.

---

🔗 Demo  
https://alee3177.github.io/kana-flashcards/

---

## ✨ 具體功能特色 Specified features

### 📘 學習內容
- 基本 50 音（あ〜ん）
- 濁音・半濁音（が / ぱ 等）
- 拗音（きゃ / しゃ 等）
- 平假名 ⇄ 片假名切換
- 羅馬拼音（Romaji）輔助顯示

### 🎴 出牌與排序模式
- 隨機（原本）
- 行內 / 段內隨機
- 行 × 段交錯（學習記憶友善）

### 🔊 聲音與操作
- 音效播放（可靜音）
- 翻面顯示答案
- 顯示答案倒數（3 秒）
- 上一張 / 下一張 / 回到第一張
- 隨機洗牌

### 🧠 學習回饋
- 「會 / 不會」標記
- 延後再出 / 稍後再出
- 清除學習紀錄
- 即時統計學習結果

---

## 📱 行動裝置最佳化（重點）

本專案**特別針對手機直式畫面（portrait）設計**：

- 上方控制區塊採 **兩欄 Grid 排版**
- 4 個 Checkbox 固定左右對齊，不會擠壓、不會變成直排文字
- 「提示 / 溫馨提醒」在手機上：
  - 顏色統一（`rgba(255,200,0,0.55)`）
  - 視覺層級一致但不搶主操作
  - 位置不影響主要操作區（已反覆驗證）

---

## ⚠️ UI 保護清單（重要）

以下區塊 **已調校完成，未來請勿隨意修改**，避免再次破壞手機版版型：

### 🚫 請勿更動
- `.controls`（上方設定區 Grid 結構）
- `.controls .footerNote`（提示 / 溫馨提醒）
- Checkbox 區塊的 HTML 結構順序
- 手機版 `@media (max-width: 768px)` 內與 controls 相關的規則

### ✅ 若需調整
- 只改「文字內容」
- 只調整 `font-size` 或 `opacity`
- 不要改 `grid-column / grid-template-columns`

---

## 🧩 技術說明

- 純 HTML / CSS / Vanilla JavaScript
- 無任何前端框架
- GitHub Pages 可直接部署
- 所有狀態皆在前端處理（不依賴後端）

---

## 📄 License

MIT License  
歡迎自由使用、修改與分享（請保留原作者資訊）