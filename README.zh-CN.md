# 🎓 SuperClaude-Tech

<div align="center">

[![Version](https://img.shields.io/badge/version-4.0.8-blue)](https://github.com/yourusername/SuperClaude-Tech)
[![License](https://img.shields.io/badge/license-MIT-green)](LICENSE)

**[English](README.md) | [简体中文](README.zh-CN.md)**

</div>

---

## 🌟 将自然语言转换为强大的SuperClaude指令

SuperClaude-Tech 是一个智能指令转换系统，将您的自然语言请求转换为精确的SuperClaude框架指令，无需记忆复杂语法即可释放Claude Code的全部潜能。

## 🎯 为什么选择SuperClaude-Tech？

SuperClaude v4框架功能极其强大，但是：
- **21个命令、14个AI代理、6个MCP服务器** - 记忆负担太大
- **不知道什么场景该用什么指令** - 选择困难，效率低下
- **新手很难掌握最佳实践** - 学习曲线陡峭

SuperClaude-Tech通过以下方式解决这些问题：
- **自然语言输入** → **最佳SuperClaude指令**
- **基于任务智能选择代理**
- **简单的`sc`激活码** - 只需记住一个暗号

## 🚀 快速开始

### 安装

1. **全局配置**
   ```bash
   # 复制CLAUDE.md到您的全局Claude Code配置
   ~/.claude/CLAUDE.md
   ```

2. **项目配置**
   ```bash
   # 或放置在项目根目录
   /your-project/CLAUDE.md
   ```

### 使用方法

只需在请求前加上`sc`：

```bash
sc 优化我的网站性能
→ /sc:troubleshoot "网站性能优化" @agent-performance-engineer --seq --think-hard
```

不加`sc`时，Claude直接执行任务：

```bash
优化我的网站性能
→ [Claude直接优化你的代码]
```

## 💡 示例

| 您的请求 | 生成的指令 |
|---------|-----------|
| `sc 网站很慢` | `/sc:troubleshoot "性能问题" @agent-performance @agent-frontend --seq` |
| `sc 做个登录系统` | `/sc:implement "认证系统" @agent-security @agent-backend --safe-mode` |
| `sc 修复这个bug` | `/sc:troubleshoot "bug修复" @agent-root-cause --verbose` |
| `sc 创建REST API` | `/sc:implement "RESTful API" @agent-backend --c7 --with-tests` |
| `sc 分析代码质量` | `/sc:analyze . @agent-quality --think-hard --focus quality` |

## 📖 文档

- **[核心配置](./docs/zh-CN/CLAUDE.md)** - 完整的提示词配置
- **[使用指南](./docs/zh-CN/GUIDE.md)** - 详细的使用说明
- **[English Docs](README.md)** - 英文文档

## 🎓 核心功能

### 21个命令
核心命令如 `/sc:implement`、`/sc:analyze`、`/sc:troubleshoot`、`/sc:improve` 等

### 14个AI代理
专业专家包括：
- `@agent-security-engineer` - 安全与认证
- `@agent-performance-engineer` - 性能优化
- `@agent-frontend-architect` - UI/UX与前端
- `@agent-backend-architect` - 后端与API
- 以及另外10个专家

### 6个MCP服务器
- `context7` - 官方文档
- `sequential-thinking` - 复杂分析
- `magic` - UI组件生成
- `playwright` - 浏览器测试
- 等等

### 智能特性
- **基于关键词的自动代理激活**
- **复杂度评估**用于最优命令选择
- **思考深度控制**（`--think`、`--think-hard`、`--think-deep`）

## 🔧 高级用法

### 组合多个代理
```bash
sc 构建安全的支付系统
→ /sc:implement "支付系统" @agent-security @agent-backend @agent-database --safe-mode --with-tests
```

### 深度分析
```bash
sc 分析架构问题
→ /sc:analyze . @agent-system-architect @agent-quality --think-deep --focus architecture
```

### 工作流自动化
```bash
sc 创建完整开发流程
→ /sc:workflow "开发流水线" @agent-devops --c7 --verbose
```

## 🎯 记住

> **想要SuperClaude指令？加 `sc`**  
> **想要直接执行？不加 `sc`**
> 
> *就这么简单！*

## 🙏 致谢

基于优秀的 [SuperClaude Framework](https://github.com/SuperClaude-Org/SuperClaude_Framework) 开发，感谢原作者的杰出贡献！

## 📝 许可证

MIT许可证 - 详见 [LICENSE](LICENSE)

## 🤝 贡献

欢迎贡献！请随时提交Pull Request。

## 👨‍💻 作者

由 黑胡子 (Blackbeard) 用 ❤️ 创建

---

<div align="center">

**[⭐ 给项目加星](https://github.com/yourusername/SuperClaude-Tech)** 如果您觉得有帮助！

</div>