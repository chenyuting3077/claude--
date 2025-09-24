# Claude 筆記

Claude AI 使用技巧和心得記錄。

## 常見用法

* 啟動：`claude`
* 初始化(建立ClAUDE.md): `/init`
* 切換至模式: `shift + tab`

## 其他指令

* `#`：更新記憶
  * e.g.: `# 請總是用繁體中文回覆`
* `@`：引用檔案內容
  * e.g.: `@ README.md`

## CLAUDE.md 

`CLAUDE.md` 是 Claude Code 的記憶檔案，讓 AI 記住你的偏好和專案相關資訊。它支援三種記憶類型，分別用於不同情境下的協作和個人專案。

### 記憶類型
| 記憶類型     | 檔案                   | 情境     |
| ------------ | ---------------------- | -------- |
| 個人記憶     | `~/.claude/CLAUDE.md	` | 所有專案 |
| 專案記憶     | `./CLAUDE.md	`         | 協作專案 |
| 本地專案記憶 | `./CLAUDE.local.md`    | 當前專案 |

## MCP 
### 基礎使用
* 加入遠端 MCP: ``` claude mcp add --transport [http|see] <name> <url> ```
  * see: 安全加密傳輸
  * http: 一般 http 傳輸
  * name: 自訂名稱
  * url: MCP 伺服器網址
  
* 查看已加入的 MCP: ``` claude mcp list ```
* 在 claude 中查詢可用 mcp: `/mcp`
    * 需要在 claude 啟動後使用

### MCP 範圍
* 加入使用範圍: `--scope <scope>`
* e.g.: `claude mcp add --transport http --scope project context7 https://mcp.context7.com/mcp` 
  
| 範圍             | 參數      | 說明               |
| ---------------- | --------- | ------------------ |
| 本地專案（預設） | `local`   | 只在當前專案可用   |
| 專案             | `project` | 在專案內所有人可用 |
| 全域             | `global`  | 在所有專案可用     |

### 常用 MCP server

| 名稱     | 用途         | Add MCP Server               |
| -------- | ------------ | ---------------------------- |
| context7 | 取得最新文件 | https://mcp.context7.com/mcp |


## 參考連結
[Claude 官方文件](https://docs.claude.com/zh-TW/docs/claude-code/mcp)

[Claude Code 技巧 教學 設定⁄指令⁄VSCode整合](https://www.youtube.com/watch?v=O9R5VwbxQdc)

[如何用 Claude Code 组建 24 小时在线的 AI Agent 员工团队](https://www.youtube.com/watch?v=QI-5-pxw-MY)

[Claude Code 的記憶大腦：CLAUDE.md 讓 AI 記住你的寫程式偏好](https://haosquare.com/claude-code-claude-md-intro/)

[Awesome Claude Code](https://github.com/hesreallyhim/awesome-claude-code)

[Claude Code MCP: How to Add MCP Servers (Complete Guide)](https://www.youtube.com/watch?v=DfWHX7kszQI)

[Claude Code PM](https://github.com/automazeio/ccpm)

[Turn Claude Code into Your Own INCREDIBLE UI Designer (using Playwright MCP Subagents)](https://www.youtube.com/watch?v=xOO8Wt_i72s)