# 🎓 SuperClaude-Tech

<div align="center">

[English](#english) | [中文](#中文)

[![Version](https://img.shields.io/badge/version-4.0.8-blue)](https://github.com/yourusername/SuperClaude-Tech)
[![License](https://img.shields.io/badge/license-MIT-green)](LICENSE)

</div>

---

## English

### 🌟 Transform Natural Language into Powerful SuperClaude Commands

SuperClaude-Tech is an intelligent instruction translation system that converts your natural language requests into precise SuperClaude Framework commands, unleashing the full potential of Claude Code without memorizing complex syntax.

### 🎯 Why SuperClaude-Tech?

The SuperClaude v4 Framework is incredibly powerful, but:
- **21 commands, 14 AI agents, 6 MCP servers** - Too much to remember
- **Context-dependent command selection** - Hard to know what to use when
- **Steep learning curve** - Difficult for beginners to master

SuperClaude-Tech solves this by:
- **Natural language input** → **Optimal SuperClaude commands**
- **Intelligent agent selection** based on your task
- **Simple `sc` activation** - Just one code to remember

### 🚀 Quick Start

1. **Install**: Copy configuration to your Claude Code
   - Global: `~/.claude/CLAUDE.md`
   - Project: `/your-project/CLAUDE.md`

2. **Use**: Just add `sc` before your request
   ```bash
   sc optimize my website performance
   → /sc:troubleshoot "website performance optimization" @agent-performance-engineer --seq --think-hard
   ```

### 📖 Documentation

- [Core Configuration](./docs/en/CLAUDE.md) - Complete prompt configuration
- [User Guide](./docs/en/GUIDE.md) - Detailed usage instructions

### 💡 Examples

| Your Request | Generated Command |
|-------------|-------------------|
| `sc my site is slow` | `/sc:troubleshoot "performance issues" @agent-performance @agent-frontend --seq` |
| `sc build login system` | `/sc:implement "auth system" @agent-security @agent-backend --safe-mode` |
| `sc fix this bug` | `/sc:troubleshoot "bug fix" @agent-root-cause --verbose` |

### 🙏 Acknowledgments

Based on the excellent [SuperClaude Framework](https://github.com/SuperClaude-Org/SuperClaude_Framework). Special thanks to the original authors!

---

## 中文

### 🌟 将自然语言转换为强大的SuperClaude指令

SuperClaude-Tech 是一个智能指令转换系统，将您的自然语言请求转换为精确的SuperClaude框架指令，无需记忆复杂语法即可释放Claude Code的全部潜能。

### 🎯 为什么选择SuperClaude-Tech？

SuperClaude v4框架功能极其强大，但是：
- **21个命令、14个AI代理、6个MCP服务器** - 记忆负担太大
- **不知道什么场景该用什么指令** - 选择困难，效率低下
- **新手很难掌握最佳实践** - 学习曲线陡峭

SuperClaude-Tech通过以下方式解决这些问题：
- **自然语言输入** → **最佳SuperClaude指令**
- **基于任务智能选择代理**
- **简单的`sc`激活码** - 只需记住一个暗号

### 🚀 快速开始

1. **安装**：复制配置到您的Claude Code
   - 全局配置：`~/.claude/CLAUDE.md`
   - 项目配置：`/项目目录/CLAUDE.md`

2. **使用**：在请求前加上`sc`即可
   ```bash
   sc 优化我的网站性能
   → /sc:troubleshoot "网站性能优化" @agent-performance-engineer --seq --think-hard
   ```

### 📖 文档

- [核心配置](./docs/zh-CN/CLAUDE.md) - 完整的提示词配置
- [使用指南](./docs/zh-CN/GUIDE.md) - 详细的使用说明

### 💡 示例

| 您的请求 | 生成的指令 |
|---------|-----------|
| `sc 网站很慢` | `/sc:troubleshoot "性能问题" @agent-performance @agent-frontend --seq` |
| `sc 做个登录系统` | `/sc:implement "认证系统" @agent-security @agent-backend --safe-mode` |
| `sc 修复这个bug` | `/sc:troubleshoot "bug修复" @agent-root-cause --verbose` |

### 🙏 致谢

基于优秀的 [SuperClaude Framework](https://github.com/SuperClaude-Org/SuperClaude_Framework) 开发，感谢原作者的杰出贡献！

---

<div align="center">

### 🎯 Remember / 记住

**English**: Want SuperClaude commands? Add `sc`  
**中文**：想要SuperClaude指令？加 `sc`

*It's that simple! / 就这么简单！*

</div>

---

## License / 许可证

MIT

## Contributing / 贡献

Contributions are welcome! Please feel free to submit a Pull Request.  
欢迎贡献！请随时提交Pull Request。

## Author / 作者

Created with ❤️ by [黑胡子]