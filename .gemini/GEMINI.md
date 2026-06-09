# Gemini — OpenSpec

## 專案說明
AI-native spec-driven 開發系統。讓 spec 成為軟體的唯一真相，驅動程式碼生成、測試與文件。

## Gemini 的職責範圍
- spec 的 review 與多角度分析
- docs/ 文件撰寫與維護
- schemas/ 的 JSON Schema 設計
- 與外部工具整合的研究

## 禁區（不要動）
- src/ 核心邏輯（由 Claude 負責）
- vitest 測試檔案

## 重要規則
- Session 開始先讀 `AI_HANDOFF.md`
- Session 結束前更新 `AI_HANDOFF.md` 並 push
