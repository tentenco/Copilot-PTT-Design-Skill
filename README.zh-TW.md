# Copilot Design Skill — by Tenten AI

**以 Copilot 為優先，專為 GitHub Copilot、ChatGPT、Codex、Claude 與 Grok 打造的創意設計 Skill。**

[English](README.md) · [繁體中文](README.zh-TW.md) · [更新紀錄](CHANGELOG.md)

![作者：Tenten AI](https://img.shields.io/badge/Author-Tenten_AI-111111) ![授權：MIT](https://img.shields.io/badge/License-MIT-2563eb) ![AI Agents](https://img.shields.io/badge/Copilot%20%C2%B7%20ChatGPT%20%C2%B7%20Codex%20%C2%B7%20Claude%20%C2%B7%20Grok-ready-7c3aed)

只要一句需求，就能把想法變成精緻、可操作的視覺作品。Copilot Design Skill 提供完整的設計流程，從方向、架構、互動式 HTML，到檢查、修改與輸出都能交給 AI Agent 完成。

它以 **GitHub Copilot** 為第一使用情境，也能在具備檔案操作能力的環境中交給 **ChatGPT、Codex、Claude 與 Grok** 使用。

## 可以做什麼

- 產品 UI、Landing Page、Dashboard 與行動裝置畫面
- 互動原型、Wireframe 與 Design System
- 簡報、文件、圖表與社群視覺
- 動畫、資料視覺化與獨立 HTML
- 可編輯 PPTX、PDF、圖片與影片輸出

## 為什麼值得用

- **一份 Brief，完成整套流程。** 從設計方向、製作、預覽到調整都由同一個 Skill 串起來。
- **以真實素材為基礎。** 可讀取截圖、HTML/CSS、程式碼、GitHub Repository 或 Figma `.fig` 檔。
- **作品留在你手上。** 產出保存在本機，可檢查、可修改，也能繼續開發。
- **不綁單一 Agent。** Copilot、ChatGPT、Codex、Claude 與 Grok 都能使用同一套流程。

> Agent 需要具備檔案讀寫權限；若要使用完整流程，建議同時提供瀏覽器預覽與終端機能力。

## 快速開始

安裝 Skill：

```bash
npx skills add tentenco/Copilot-PTT-Design-Skill
```

或請你的 AI Agent 直接讀取 Skill 的入口檔案：

```text
請讀取 skills/copilot-design/SKILL.md 並依照其中流程，為個人理財 Dashboard
設計三個高保真方向，最後輸出為獨立 HTML。
```

若要手動安裝，可將 [`skills/copilot-design/`](skills/copilot-design/) 複製到 Agent 支援的 Skills 目錄，流程會從 `SKILL.md` 開始。

## 運作方式

```text
你的 Brief → 設計方法 → 任務 Skill → 互動式 HTML → 檢查調整 → 輸出
```

入口 Skill 只會載入當下任務需要的內容。內建流程涵蓋高保真 UI、互動原型、簡報、文件、動態設計、研究、Design System、素材匯入與正式輸出。

所有能力都整理在同一個可攜式套件中：

```text
skills/copilot-design/
├── SKILL.md              # 從這裡開始
├── system-prompt.md      # 設計方法與品質標準
├── built-in-skills/      # 任務專用流程
├── starter-components/   # 可重複使用的視覺元件
├── references/           # 各 Agent 的工具指引
└── agents/               # 匯入、驗證與輸出工具
```

## Prompt 靈感

```text
參考這張截圖的視覺語言，設計一個重點清楚的 SaaS Landing Page。
```

```text
把這份產品 Brief 做成可互動的 App Onboarding Prototype。
```

```text
製作一份 10 頁募資簡報，加入原生進場動畫，並輸出為可編輯 PPTX。
```

```text
把這份 Figma 檔匯入成 Design System，再用它設計 Analytics Dashboard。
```

## 支援你的 AI 工作流

| Agent | 建議用途 |
|---|---|
| **GitHub Copilot** | 核心使用情境，Copilot-first 工作流 |
| **ChatGPT** | 在可操作檔案的程式開發環境中設計與製作 |
| **Codex** | 本機實作、預覽、驗證與輸出 |
| **Claude** | 設計探索與視覺作品製作 |
| **Grok** | 在具備檔案工具的環境中依 Prompt 建立作品 |

## 作者與授權

由 **Tenten AI** 重新定位並維護。

本專案將 Claude Design 的方法轉化為可攜式 AI Agent 工作流，為獨立專案，與 Anthropic、GitHub、OpenAI、xAI 或其產品皆無從屬或背書關係。原有上游版權聲明仍然有效，並依 [MIT License](LICENSE) 發布。
