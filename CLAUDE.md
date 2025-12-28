# CLAUDE.md

此檔案為 Claude Code (claude.ai/code) 在此程式庫中工作時提供指引。

## 程式庫概述

這是一個專為 Claude Code 設計的專業 AI 代理與技能集合，針對快速的 6 天衝刺開發週期進行優化。此專案採用混合架構：

- **代理 (Agents)**：獨立執行任務的子代理，適合需要工具操作的執行型任務
- **技能 (Skills)**：提供專業知識和指南，Claude 可根據上下文自動運用

## 架構說明

### 代理 (Agents)
代理是帶有 YAML 前置資料的 Markdown 檔案，可獨立執行任務：

```yaml
---
name: agent-name              # kebab-case 識別碼
description: ...              # 使用時機 + 4 個帶有 <example> 標籤的範例
color: green                  # 視覺識別顏色
tools: Write, Read, Bash, ... # 代理可使用的工具
---

[系統提示：500 字以上，定義代理行為、職責和專業領域]
```

適合作為代理的任務：
- 程式碼實作與修改
- 測試執行與修復
- 部署與 DevOps 操作
- UI/UX 實作

### 技能 (Skills)
技能位於 `.claude/skills/` 目錄，提供專業知識供 Claude 參考：

```
.claude/skills/
├── brand-guidelines/SKILL.md      # 品牌設計指南
├── ux-research/SKILL.md           # UX 研究方法
├── visual-storytelling/SKILL.md   # 視覺敘事
├── trend-research/SKILL.md        # 趨勢研究
├── feedback-analysis/SKILL.md     # 回饋分析
├── sprint-prioritization/SKILL.md # 衝刺優先順序
├── aso-optimization/SKILL.md      # 應用商店優化
├── content-creation/SKILL.md      # 內容創作
├── growth-hacking/SKILL.md        # 成長駭客
├── analytics-insights/SKILL.md    # 分析洞察
├── legal-compliance/SKILL.md      # 法律合規
├── tool-evaluation/SKILL.md       # 工具評估
└── workflow-optimization/SKILL.md # 工作流程優化
```

適合作為技能的任務：
- 提供專業知識和最佳實踐
- 指南和框架參考
- 決策支援和建議

## 部門組織

### 代理目錄
- `engineering/` - 程式碼實作、測試、DevOps、原型開發
- `design/` - UI 設計、趣味注入
- `marketing/` - 社群平台互動、社群經營
- `product/` - （已轉為技能）
- `project-management/` - 衝刺管理、產品發布、實驗
- `studio-operations/` - 財務、基礎設施、支援
- `testing/` - API 測試、效能基準
- `bonus/` - 特殊代理（studio-coach、joker）

### 技能目錄
- `.claude/skills/` - 所有知識型技能

## 核心概念

**6 天衝刺**：所有代理與技能皆針對快速開發週期進行優化。

**主動式代理**：部分代理會自動觸發：
- `studio-coach` - 複雜的多代理任務或代理需要指導時
- `test-writer-fixer` - 功能實作、錯誤修復或程式碼修改後
- `whimsy-injector` - UI/UX 變更後
- `experiment-tracker` - 新增功能旗標時

**多代理協作**：代理設計為可協同工作。複雜任務通常受益於多個專家的合作。

**技能自動運用**：Claude 會根據對話上下文自動參考相關技能的知識。

## 新增/修改代理

建立或修改代理時：

1. 在描述中使用 `<example>`、`<commentary>` 標籤格式
2. 包含 3-4 個詳細範例，展示情境、使用者輸入和助手回應
3. 撰寫 500 字以上的系統提示，涵蓋：
   - 代理身份與角色
   - 5-8 項主要職責（含編號子項目）
   - 不同情境的決策框架
   - 最佳實踐與錯誤處理
4. 工具應符合代理的能力（Write、MultiEdit、Bash、Read、Glob、Task 等）

## 新增/修改技能

建立技能時：

1. 在 `.claude/skills/` 下建立新目錄
2. 建立 `SKILL.md` 檔案
3. 內容應包含：
   - 清晰的標題和說明
   - 核心原則和框架
   - 最佳實踐和範例
   - 檢查清單和範本
4. 技能應專注於「如何做」而非「執行什麼」

## 安裝位置

- 代理安裝至 `~/.claude/agents/`
- 技能安裝至 `~/.claude/skills/`（或專案內的 `.claude/skills/`）
