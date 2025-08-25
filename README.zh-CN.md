# SuperClaude-Tech

<div align="center">

[![Version](https://img.shields.io/badge/version-4.0.8-blue)](https://github.com/heihuzicity-tech/SuperClaude-Tech)
[![License](https://img.shields.io/badge/license-MIT-green)](LICENSE)

**[English](README.md) | [简体中文](README.zh-CN.md)**

</div>

---

## SuperClaude-Tech 是什么？

SuperClaude-Tech 是一个智能命令生成器，它将自然语言转换为专业的 SuperClaude Framework 命令。无需记忆复杂语法，让每个人都能轻松使用强大的 SuperClaude Framework。

## 面临的问题

SuperClaude Framework v4 提供了 21 个命令、14 个 AI 代理和几十个标志。一个典型的命令如下：

```bash
/sc:implement "用户认证" @agent-security-engineer @agent-backend-architect --c7 --safe-mode --with-tests --validate
```

**你能记住所有这些吗：**
- 精确的命令名称？
- 每个任务该用哪些代理？
- 必需的标志及其组合？
- 正确的语法和顺序？

大多数开发者记不住，也不应该去记。

## 解决方案

使用 SuperClaude-Tech，你只需输入：

```bash
sc 构建一个安全的登录系统
```

立即获得包含所有必要组件的完整优化命令。

## 核心价值

### 1. 零记忆负担
- 只需记住 `sc`，而不是 21 个命令 + 14 个代理 + 几十个标志
- 使用自然语言，而非技术语法
- 无需不断查阅文档

### 2. 内置最佳实践
- 自动为你的任务选择合适的代理
- 包含必要的安全和质量标志
- 遵循官方 SuperClaude 模式

### 3. 学习工具
- 准确了解每个任务使用哪些命令和代理
- 通过观察学习，而非死记硬背
- 在使用中逐步理解框架

## 前置要求

SuperClaude-Tech 需要先安装 **SuperClaude Framework**。这是一个基于 SuperClaude 之上的增强工具。

### 安装 SuperClaude Framework

```bash
# 推荐：使用 pipx 安装
pipx install SuperClaude && SuperClaude install

# 或使用 pip
pip install SuperClaude && SuperClaude install

# 或使用 npm
npm install -g @bifrost_inc/superclaude && superclaude install
```

详细安装说明请访问 [SuperClaude Framework](https://github.com/SuperClaude-Org/SuperClaude_Framework) 仓库。

## 安装

安装 SuperClaude Framework 后，安装 SuperClaude-Tech：

```bash
# 将 CLAUDE.md 放置在 Claude Code 配置目录
~/.claude/CLAUDE.md

# 或放在项目根目录
/your-project/CLAUDE.md
```

## 使用方法

### 基本用法

在任何请求前添加 `sc` 来生成命令：

```bash
# 输入
sc 优化数据库性能

# 输出
/sc:improve "数据库性能" @agent-backend-architect @agent-performance-engineer --seq --ultrathink --systematic
```

### 真实示例

| 自然语言 | 生成的专业命令 |
|---------|--------------|
| `sc 修复内存泄漏` | `/sc:troubleshoot "内存泄漏" @agent-performance-engineer @agent-root-cause-analyst --trace --verbose --safe-mode` |
| `sc 构建购物车` | `/sc:implement "购物车" @agent-backend-architect @agent-frontend-architect --c7 --magic --with-tests --validate` |
| `sc 审计安全性` | `/sc:analyze . @agent-security-engineer --focus security --systematic --validate --trace` |
| `sc 重构遗留代码` | `/sc:improve "遗留代码重构" @agent-refactoring-expert @agent-system-architect --wave-mode force --wave-strategy enterprise --systematic` |

## 谁会受益？

### 初学者
- 无需学习语法即可立即使用 SuperClaude
- 专注于想要实现的目标，而不是如何表达
- 通过生成的示例自然地学习框架

### 经验丰富的开发者
- 快速查询复杂的命令组合
- 永远不会忘记很少使用的标志或代理名称
- 确保团队项目的一致性

### 团队
- 在整个组织中标准化命令模式
- 减少新成员的入职时间
- 自动维护最佳实践

## 功能特性

### 智能代理选择
自动识别你需要的专家：
- 安全任务 → `@agent-security-engineer`
- 性能问题 → `@agent-performance-engineer`
- UI 组件 → `@agent-frontend-architect`
- 系统设计 → `@agent-system-architect`

### 智能标志组合
根据上下文应用适当的标志：
- 生产代码 → `--safe-mode --validate`
- 复杂分析 → `--seq --ultrathink --systematic`
- 需要测试 → `--with-tests --coverage`

### 复杂度评估
自动判断任务复杂度并添加：
- 大规模操作的 Wave 模式
- 提高效率的并行执行标记
- 多步骤任务的 TodoWrite 建议

## 文档

- **[核心配置](./docs/zh-CN/CLAUDE.md)** - 完整系统文档
- **[使用指南](./docs/zh-CN/GUIDE.md)** - 详细使用示例
- **[English Docs](README.md)** - 英文文档

## 技术细节

### 支持的组件
- **21 个命令**：implement、analyze、troubleshoot、improve、test、build、design 等
- **14 个 AI 代理**：从安全工程师到前端架构师
- **6 个 MCP 服务器**：文档、分析、UI 生成、测试工具
- **5 种行为模式**：头脑风暴、任务管理、编排等

### 工作原理
1. 你用自然语言描述需求
2. SuperClaude-Tech 分析你的意图
3. 它选择合适的命令、代理和标志
4. 返回完整的、可直接使用的 SuperClaude 命令

## 贡献

欢迎贡献！请随时提交 Pull Request。

## 许可证

MIT 许可证 - 详见 [LICENSE](LICENSE)

## 致谢

基于 [SuperClaude Framework](https://github.com/SuperClaude-Org/SuperClaude_Framework) 构建。感谢原作者创建了如此强大的工具。

## 作者

由黑胡子 (Blackbeard) 创建

网站：[https://www.heihuzicity.com/](https://www.heihuzicity.com/)

---

<div align="center">

**[为这个项目点星](https://github.com/heihuzicity-tech/SuperClaude-Tech)** 如果你觉得有帮助！

</div>