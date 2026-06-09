# Gemini — OpenSpec

## 專案說明
AI-native spec-driven 開發系統。讓 spec 成為軟體的唯一真相，驅動程式碼生成、測試與文件。

## 技術棧
- TypeScript + Node.js\n- Vitest 測試\n- Bun / pnpm

## 開發慣例
- 所有新功能先寫 spec，再實作\n- 測試覆蓋率維持在合理水準\n- dist/ 不手動修改

## 不要手動修改的檔案（自動產生）
- dist/（build 產出）\n- node_modules/\n- pnpm-lock.yaml / bun.lock（不手動修改）

## Handoff 協議
- **Session 開始**：先 `git pull`，再讀 `AI_HANDOFF.md` 了解目前進度與誰在負責哪個檔案
- **Session 進行中**：若要動某個檔案，先確認 AI_HANDOFF.md 裡沒有 🔒 標記
- **Session 結束**：在 `AI_HANDOFF.md` 最上方新增記錄，移除自己的 🔒，commit & push

### AI_HANDOFF.md 記錄格式
```
## YYYY-MM-DD | Gemini | 家裡／公司
- 完成：（做了什麼）
- 下次：（下個 session 要繼續的）
- 🔒 進行中：（還沒 push 完的檔案，請另一個 AI 暫勿修改）
```
