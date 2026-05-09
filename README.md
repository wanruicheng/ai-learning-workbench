# 本科 AI 学习工作台：Claude Code / Codex / MCP 配置方案

这是一个面向本科阶段的 AI 学习工作流展示页，主要用于记录和分享个人的 Claude Code 桌面端配置方案。

## 项目内容

- Claude 桌面端 + DeepSeek 使用分工
- PowerShell Claude Code 备用与排错入口
- Codex 桌面端用于 Python / 项目调试
- Tavily MCP 用于联网资料检索
- 百度地图 MCP 用于国内地点、路线和距离查询
- AI-Sandbox 安全文件区
- Skills 下载区
- 实验报告、课程作业、Python 学习、旅游规划工作流
- 常用 Prompt 一键复制

## 文件结构

```text
index.html
skills/
README.md
SECURITY.md
CHANGELOG.md
.nojekyll
```

## 使用方式

直接打开 `index.html` 即可本地查看。

如果移动文件，请保持 `skills/` 文件夹和 `index.html` 在同一目录，否则 Skill 下载链接会失效。

## 公开前检查

不要公开以下内容：

- API Key
- 账号、手机号
- 密钥截图
- 私人路径和隐私文件
- 包含真实 token 的配置文件

## 项目定位

这个项目不是复杂前端项目，而是一个真实可用的 AI 学习工作流展示页。重点是工具组合、任务流程和安全边界。


## 从零配置摘要

1. 建立固定工作区：`Desktop/Code`、`AI-Sandbox/input`、`output`、`backup`、`temp`
2. 安装并检查 Claude Code：`claude --version`
3. 配置认证：根据官方 API 或第三方网关设置对应环境变量
4. 写入长期指令：`%USERPROFILE%\.claude\CLAUDE.md`
5. 安装 Skills：本地放入 `.claude/skills`，桌面端上传 ZIP
6. 添加 MCP：优先 Remote MCP，例如 Tavily、百度地图 MCP
7. 做最小测试：docx、Tavily、百度地图、/status、/mcp

## 官方文档

- Claude Code Settings: https://code.claude.com/docs/en/settings
- Environment Variables: https://code.claude.com/docs/en/env-vars
- Authentication: https://code.claude.com/docs/en/authentication

## Claude 界面中文化

本项目只提供社区汉化项目入口，不直接分发汉化包。使用前请自行检查项目来源、安装脚本和安全风险。

参考：
- https://github.com/javaht/claude-desktop-zh-cn
- https://github.com/pheohu-42/Claude_zh-CN_LanguagePack
- https://github.com/Jyy1529/claude-desktop_win-zh_cn

## 新手友好版说明

v10 增加了以下内容：

- 新手前置须知
- 小白术语词典
- 10 分钟入门案例
- Skill 极简使用卡片
- 高频排错指南

目标是让从未接触过 Claude Code / MCP / Skills 的用户，也能理解这套系统应该从哪里开始。

## v11 完整新手教程

本版进一步补齐“新手入门最后一公里”：

- 新手零门槛前置准备
- Key / AK 申请说明
- 安装命令的预期效果与失败排查
- Windows / macOS 操作差异
- Skill 桌面端与 Claude Code 两种安装方式
- Prompt 使用场景说明
- 更完整的新手高频排错

## v12 细节收尾版

本版主要做最终 polish：

- 修正百度地图 MCP 命令说明
- 补充 Codex 术语解释
- 优化 10 分钟案例的复制提示
- 优化步骤文本可读性
- 补充下载链接实测提醒

## v13 精简收尾版

- 删除页面末尾的“后续维护建议”
- 删除独立的“公开前检查清单”
- 将公开安全提醒压缩合并到安全板块中

## v14 新手导航优化版

- 新增“我该从哪开始？”入口
- 将 10 分钟案例优化为“5～10 分钟新手试跑”
- 新增国内用户使用说明
- 新增纯小白 FAQ 三问
- 优化首页按钮跳转目标

## v15 远程控制与 Subagents 版

本版新增：

- 微信 + cc-connect + Claude Code 远程控制说明
- 远程安全规则
- 微信远程常用提示词
- Subagents 说明：security-reviewer、project-maintainer、study-file-planner
- Hooks 路线建议：先设计方案，不急着启用

## v16 cc-connect 微信远程教程版

- 补充 cc-connect 接入微信完整流程
- 新增项目设置建议：Claudecode、工作目录、plan 模式
- 新增 localhost / PATH / 微信重绑等常见排错
- 扩充微信远程常用提示词收藏

## v17 远程安全与 Subagents / Hooks 版

本版新增：

- 远程安全规则完整板块
- 可复制的微信远程安全前缀
- Subagents 配置说明与创建提示词
- security-reviewer / project-maintainer / study-file-planner 测试指令
- Hooks 安全方案说明：先设计，不急着启用
