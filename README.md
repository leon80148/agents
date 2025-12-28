# Claude Code 專業代理與技能集合

> 🙏 **致謝**：本專案改編自 [Contains Studio](https://github.com/contains-studio/agents) 的原始代理集合。感謝他們提供優秀的基礎架構。

這是一個專為 Claude Code 設計的專業 AI 代理與技能集合，針對快速的 6 天衝刺開發週期進行優化。專案採用混合架構，結合執行型代理與知識型技能，以最大化開發效率。

## 📥 安裝

1. **下載此程式庫：**
   ```bash
   git clone https://github.com/[your-username]/agents.git
   ```

2. **複製代理到 Claude Code 目錄：**
   ```bash
   # 複製代理
   cp -r agents/engineering ~/.claude/agents/
   cp -r agents/design ~/.claude/agents/
   cp -r agents/marketing ~/.claude/agents/
   cp -r agents/project-management ~/.claude/agents/
   cp -r agents/studio-operations ~/.claude/agents/
   cp -r agents/testing ~/.claude/agents/
   cp -r agents/bonus ~/.claude/agents/

   # 複製技能
   cp -r agents/.claude/skills ~/.claude/
   ```

3. **重新啟動 Claude Code** 以載入新的代理和技能。

## 🏗️ 架構說明

本專案採用混合架構：

### 代理 (Agents) - 執行型
獨立的子代理，可使用工具執行任務：
- 程式碼實作與修改
- 測試執行與修復
- 部署與 DevOps 操作
- UI/UX 實作

### 技能 (Skills) - 知識型
提供專業知識和最佳實踐供 Claude 參考：
- 品牌設計指南
- UX 研究方法
- 成長駭客策略
- 法律合規檢查

## 📁 目錄結構

```
agents/
├── .claude/
│   └── skills/                    # 知識型技能
│       ├── brand-guidelines/      # 品牌設計指南
│       ├── ux-research/           # UX 研究方法
│       ├── visual-storytelling/   # 視覺敘事
│       ├── trend-research/        # 趨勢研究
│       ├── feedback-analysis/     # 回饋分析
│       ├── sprint-prioritization/ # 衝刺優先順序
│       ├── aso-optimization/      # 應用商店優化
│       ├── content-creation/      # 內容創作
│       ├── growth-hacking/        # 成長駭客
│       ├── analytics-insights/    # 分析洞察
│       ├── legal-compliance/      # 法律合規
│       ├── tool-evaluation/       # 工具評估
│       └── workflow-optimization/ # 工作流程優化
├── engineering/                   # 工程代理
│   ├── ai-engineer.md
│   ├── backend-architect.md
│   ├── devops-automator.md
│   ├── frontend-developer.md
│   ├── mobile-app-builder.md
│   ├── rapid-prototyper.md
│   └── test-writer-fixer.md
├── design/                        # 設計代理
│   ├── ui-designer.md
│   └── whimsy-injector.md
├── marketing/                     # 行銷代理
│   ├── instagram-curator.md
│   ├── reddit-community-builder.md
│   ├── tiktok-strategist.md
│   └── twitter-engager.md
├── project-management/            # 專案管理代理
│   ├── experiment-tracker.md
│   ├── project-shipper.md
│   └── studio-producer.md
├── studio-operations/             # 工作室營運代理
│   ├── finance-tracker.md
│   ├── infrastructure-maintainer.md
│   └── support-responder.md
├── testing/                       # 測試代理
│   ├── api-tester.md
│   ├── performance-benchmarker.md
│   └── test-results-analyzer.md
└── bonus/                         # 特殊代理
    ├── studio-coach.md
    └── joker.md
```

## 📋 代理清單

### 工程部門 (`engineering/`)
| 代理 | 說明 |
|------|------|
| ai-engineer | 整合實際可發布的 AI/ML 功能 |
| backend-architect | 設計可擴展的 API 和伺服器系統 |
| devops-automator | 持續部署而不破壞系統 |
| frontend-developer | 建構極速的使用者介面 |
| mobile-app-builder | 建立原生 iOS/Android 體驗 |
| rapid-prototyper | 在數天內建構 MVP |
| test-writer-fixer | 撰寫能捕捉真實錯誤的測試 |

### 設計部門 (`design/`)
| 代理 | 說明 |
|------|------|
| ui-designer | 設計開發者能實際建構的介面 |
| whimsy-injector | 為每個互動添加趣味 |

### 行銷部門 (`marketing/`)
| 代理 | 說明 |
|------|------|
| instagram-curator | 精通視覺內容策略 |
| reddit-community-builder | 在 Reddit 上建立社群 |
| tiktok-strategist | 創造可分享的行銷時刻 |
| twitter-engager | 利用趨勢獲得病毒式互動 |

### 專案管理 (`project-management/`)
| 代理 | 說明 |
|------|------|
| experiment-tracker | 數據驅動的功能驗證 |
| project-shipper | 發布不會崩潰的產品 |
| studio-producer | 讓團隊專注於發布，而非開會 |

### 工作室營運 (`studio-operations/`)
| 代理 | 說明 |
|------|------|
| finance-tracker | 保持工作室盈利 |
| infrastructure-maintainer | 擴展而不增加成本 |
| support-responder | 將不滿的使用者轉變為擁護者 |

### 測試 (`testing/`)
| 代理 | 說明 |
|------|------|
| api-tester | 確保 API 在壓力下正常運作 |
| performance-benchmarker | 讓一切更快 |
| test-results-analyzer | 從測試失敗中找出模式 |

### 特殊代理 (`bonus/`)
| 代理 | 說明 |
|------|------|
| studio-coach | 召集 AI 團隊達到卓越 |
| joker | 用科技幽默緩和氣氛 |

## 📚 技能清單

| 技能 | 說明 |
|------|------|
| brand-guidelines | 品牌設計、視覺識別系統指南 |
| ux-research | UX 研究方法與使用者行為分析 |
| visual-storytelling | 視覺敘事、資訊圖表設計 |
| trend-research | 市場趨勢分析與機會識別 |
| feedback-analysis | 使用者回饋分析與洞察 |
| sprint-prioritization | 衝刺規劃與優先順序排定 |
| aso-optimization | 應用商店優化策略 |
| content-creation | 跨平台內容創作 |
| growth-hacking | 成長駭客策略與實驗 |
| analytics-insights | 數據分析與效能報告 |
| legal-compliance | 法規合規與隱私政策 |
| tool-evaluation | 開發工具評估框架 |
| workflow-optimization | 工作流程優化與自動化 |

## 🎯 主動式代理

部分代理會在特定情境下自動觸發：

- **studio-coach** - 複雜的多代理任務開始時或代理需要指導時
- **test-writer-fixer** - 實作功能、修復錯誤或修改程式碼後
- **whimsy-injector** - UI/UX 變更後
- **experiment-tracker** - 新增功能旗標時

## 💡 最佳實踐

1. **讓代理協同工作** - 許多任務受益於多個代理合作
2. **具體描述** - 清晰的任務描述幫助代理表現更好
3. **信任專業** - 代理專為其特定領域設計
4. **快速迭代** - 代理支援 6 天衝刺理念
5. **運用技能** - 技能提供的知識可指導決策

## 🤝 貢獻

歡迎改進現有代理或建議新代理：

1. 使用現有格式建立新的 `.md` 檔案
2. 包含 3-4 個詳細的使用範例
3. 撰寫全面的系統提示（500 字以上）
4. 以真實任務測試代理

## 📄 授權

本專案改編自 [Contains Studio Agents](https://github.com/contains-studio/agents)。

---

**🔗 相關連結**
- [Claude Code 子代理文件](https://docs.anthropic.com/en/docs/claude-code/sub-agents)
- [原始專案：Contains Studio Agents](https://github.com/contains-studio/agents)
