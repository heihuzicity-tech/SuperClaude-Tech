# 🎓 SuperClaude-Tech

<div align="center">

[![Version](https://img.shields.io/badge/version-4.0.8-blue)](https://github.com/yourusername/SuperClaude-Tech)
[![License](https://img.shields.io/badge/license-MIT-green)](LICENSE)

**[English](README.md) | [简体中文](README.zh-CN.md)**

</div>

---

## 🌟 Transform Natural Language into Powerful SuperClaude Commands

SuperClaude-Tech is an intelligent instruction translation system that converts your natural language requests into precise SuperClaude Framework commands, unleashing the full potential of Claude Code without memorizing complex syntax.

## 🎯 Why SuperClaude-Tech?

The SuperClaude v4 Framework is incredibly powerful, but:
- **21 commands, 14 AI agents, 6 MCP servers** - Too much to remember
- **Context-dependent command selection** - Hard to know what to use when
- **Steep learning curve** - Difficult for beginners to master

SuperClaude-Tech solves this by:
- **Natural language input** → **Optimal SuperClaude commands**
- **Intelligent agent selection** based on your task
- **Simple `sc` activation** - Just one code to remember

## 🚀 Quick Start

### Installation

1. **Global Configuration**
   ```bash
   # Copy CLAUDE.md to your global Claude Code config
   ~/.claude/CLAUDE.md
   ```

2. **Project Configuration**
   ```bash
   # Or place it in your project root
   /your-project/CLAUDE.md
   ```

### Usage

Just add `sc` before your request:

```bash
sc optimize my website performance
→ /sc:troubleshoot "website performance optimization" @agent-performance-engineer --seq --think-hard
```

Without `sc`, Claude executes tasks directly:

```bash
optimize my website performance
→ [Claude directly optimizes your code]
```

## 💡 Examples

| Your Request | Generated Command |
|-------------|-------------------|
| `sc my site is slow` | `/sc:troubleshoot "performance issues" @agent-performance @agent-frontend --seq` |
| `sc build login system` | `/sc:implement "auth system" @agent-security @agent-backend --safe-mode` |
| `sc fix this bug` | `/sc:troubleshoot "bug fix" @agent-root-cause --verbose` |
| `sc create REST API` | `/sc:implement "RESTful API" @agent-backend --c7 --with-tests` |
| `sc analyze code quality` | `/sc:analyze . @agent-quality --think-hard --focus quality` |

## 📖 Documentation

- **[Core Configuration](./docs/en/CLAUDE.md)** - Complete prompt configuration
- **[User Guide](./docs/en/GUIDE.md)** - Detailed usage instructions
- **[中文文档](README.zh-CN.md)** - Chinese documentation

## 🎓 Key Features

### 21 Commands
Core commands like `/sc:implement`, `/sc:analyze`, `/sc:troubleshoot`, `/sc:improve`, and more

### 14 AI Agents
Specialized experts including:
- `@agent-security-engineer` - Security & authentication
- `@agent-performance-engineer` - Performance optimization
- `@agent-frontend-architect` - UI/UX & frontend
- `@agent-backend-architect` - Backend & APIs
- And 10 more specialists

### 6 MCP Servers
- `context7` - Official documentation
- `sequential-thinking` - Complex analysis
- `magic` - UI component generation
- `playwright` - Browser testing
- And more

### Intelligent Features
- **Auto-agent activation** based on keywords
- **Complexity assessment** for optimal command selection
- **Thinking depth control** (`--think`, `--think-hard`, `--think-deep`)

## 🔧 Advanced Usage

### Combining Multiple Agents
```bash
sc build secure payment system
→ /sc:implement "payment system" @agent-security @agent-backend @agent-database --safe-mode --with-tests
```

### Deep Analysis
```bash
sc analyze architecture problems
→ /sc:analyze . @agent-system-architect @agent-quality --think-deep --focus architecture
```

### Workflow Automation
```bash
sc create full development workflow
→ /sc:workflow "development pipeline" @agent-devops --c7 --verbose
```

## 🎯 Remember

> **Want SuperClaude commands? Add `sc`**  
> **Want direct execution? No `sc`**
> 
> *It's that simple!*

## 🙏 Acknowledgments

Based on the excellent [SuperClaude Framework](https://github.com/SuperClaude-Org/SuperClaude_Framework). Special thanks to the original authors for their outstanding contribution!

## 📝 License

MIT License - See [LICENSE](LICENSE) for details

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 👨‍💻 Author

Created with ❤️ by 黑胡子 (Blackbeard)

🌐 Website: [https://www.heihuzicity.com/](https://www.heihuzicity.com/)

---

<div align="center">

**[⭐ Star this project](https://github.com/yourusername/SuperClaude-Tech)** if you find it helpful!

</div>