# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Overview

這是一個 Claude AI 使用技巧和心得記錄的個人筆記倉庫，使用繁體中文維護。作為 Claude AI 最佳實踐和常見使用模式的參考指南。

## Repository Structure

- `README.md` - 包含 Claude AI 使用技巧、常見指令、MCP 設定和參考連結的主要文件
- 無建置系統、測試或開發相依性的純文件倉庫

## Key Content Areas

### Claude 基礎操作
- 啟動指令：`claude`
- 初始化指令：`/init`
- 模式切換：`shift + tab`
- 記憶更新：`#` (例如：`# 請總是用繁體中文回覆`)
- 檔案引用：`@` (例如：`@ README.md`)

### CLAUDE.md 記憶系統
支援三種記憶類型：
- 個人記憶 (`~/.claude/CLAUDE.md`) - 適用所有專案
- 專案記憶 (`./CLAUDE.md`) - 適用協作專案
- 本地專案記憶 (`./CLAUDE.local.md`) - 適用當前專案

### MCP (Model Context Protocol) 配置
- 新增 MCP 伺服器：`claude mcp add --transport [http|see] <name> <url>`
- 查看已加入的 MCP：`claude mcp list`
- 在 Claude 中查詢：`/mcp`
- 範圍設定：`--scope <local|project|global>`

## Communication Preferences

- 請總是用繁體中文回覆
- 專注於 Claude AI 使用技巧和最佳實踐
- 維護文件的實用性和可讀性