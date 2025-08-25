# SuperClaude-Tech

<div align="center">

[![Version](https://img.shields.io/badge/version-4.0.8-blue)](https://github.com/heihuzicity-tech/SuperClaude-Tech)
[![License](https://img.shields.io/badge/license-MIT-green)](LICENSE)

**[English](README.md) | [简体中文](README.zh-CN.md)**

</div>

---

## What is SuperClaude-Tech?

SuperClaude-Tech is an intelligent command generator that converts natural language into professional SuperClaude Framework commands. It eliminates the need to memorize complex syntax, making the powerful SuperClaude Framework accessible to everyone.

## The Problem

SuperClaude Framework v4 provides 21 commands, 14 AI agents, and dozens of flags. A typical command looks like this:

```bash
/sc:implement "user authentication" @agent-security-engineer @agent-backend-architect --c7 --safe-mode --with-tests --validate
```

**Can you remember all the:**
- Exact command names?
- Which agents to use for each task?
- Required flags and their combinations?
- Correct syntax and order?

Most developers can't, and shouldn't have to.

## The Solution

With SuperClaude-Tech, you simply type:

```bash
sc build a secure login system
```

And instantly get the complete, optimized command with all necessary components.

## Key Benefits

### 1. Zero Memory Burden
- Remember just `sc` instead of 21 commands + 14 agents + dozens of flags
- Use natural language, not technical syntax
- No need to check documentation constantly

### 2. Best Practices Built-in
- Automatically selects appropriate agents for your task
- Includes necessary security and quality flags
- Follows official SuperClaude patterns

### 3. Learning Tool
- See exactly which commands and agents are used for each task
- Learn by observation, not memorization
- Gradually understand the framework through usage

## Prerequisites

SuperClaude-Tech requires the **SuperClaude Framework** to be installed first. This is an enhancement tool that works on top of SuperClaude.

### Install SuperClaude Framework

```bash
# Recommended: Install using pipx
pipx install SuperClaude && SuperClaude install

# Or using pip
pip install SuperClaude && SuperClaude install

# Or using npm
npm install -g @bifrost_inc/superclaude && superclaude install
```

For detailed installation instructions, visit the [SuperClaude Framework](https://github.com/SuperClaude-Org/SuperClaude_Framework) repository.

## Installation

After installing SuperClaude Framework, install SuperClaude-Tech:

```bash
# Place CLAUDE.md in your Claude Code configuration
~/.claude/CLAUDE.md

# Or in your project root
/your-project/CLAUDE.md
```

## Usage

### Basic Usage

Add `sc` before any request to generate the command:

```bash
# Input
sc optimize database performance

# Output
/sc:improve "database performance" @agent-backend-architect @agent-performance-engineer --seq --ultrathink --systematic
```

### Real-World Examples

| Natural Language | Generated Professional Command |
|-----------------|-------------------------------|
| `sc fix memory leak` | `/sc:troubleshoot "memory leak" @agent-performance-engineer @agent-root-cause-analyst --trace --verbose --safe-mode` |
| `sc build shopping cart` | `/sc:implement "shopping cart" @agent-backend-architect @agent-frontend-architect --c7 --magic --with-tests --validate` |
| `sc audit security` | `/sc:analyze . @agent-security-engineer --focus security --systematic --validate --trace` |
| `sc refactor legacy code` | `/sc:improve "legacy code refactoring" @agent-refactoring-expert @agent-system-architect --wave-mode force --wave-strategy enterprise --systematic` |

## Who Benefits?

### Beginners
- Start using SuperClaude immediately without learning syntax
- Focus on what you want to achieve, not how to phrase it
- Learn the framework naturally through generated examples

### Experienced Developers
- Quick reference for complex command combinations
- Never forget rarely-used flags or agent names
- Ensure consistency across team projects

### Teams
- Standardize command patterns across the organization
- Reduce onboarding time for new members
- Maintain best practices automatically

## Features

### Smart Agent Selection
Automatically identifies which experts you need:
- Security tasks → `@agent-security-engineer`
- Performance issues → `@agent-performance-engineer`
- UI components → `@agent-frontend-architect`
- System design → `@agent-system-architect`

### Intelligent Flag Combination
Applies appropriate flags based on context:
- Production code → `--safe-mode --validate`
- Complex analysis → `--seq --ultrathink --systematic`
- Testing required → `--with-tests --coverage`

### Complexity Assessment
Automatically determines task complexity and adds:
- Wave modes for large-scale operations
- Parallel execution markers for efficiency
- TodoWrite suggestions for multi-step tasks

## Documentation

- **[Core Configuration](./docs/en/CLAUDE.md)** - Complete system documentation
- **[User Guide](./docs/en/GUIDE.md)** - Detailed usage examples
- **[中文文档](README.zh-CN.md)** - Chinese documentation

## Technical Details

### Supported Components
- **21 Commands**: implement, analyze, troubleshoot, improve, test, build, design, and more
- **14 AI Agents**: From security engineers to frontend architects
- **6 MCP Servers**: Documentation, analysis, UI generation, testing tools
- **5 Behavior Modes**: Brainstorming, Task Management, Orchestration, and more

### How It Works
1. You describe what you want in natural language
2. SuperClaude-Tech analyzes your intent
3. It selects appropriate commands, agents, and flags
4. Returns the complete, ready-to-use SuperClaude command

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

MIT License - See [LICENSE](LICENSE) for details

## Acknowledgments

Built on top of the [SuperClaude Framework](https://github.com/SuperClaude-Org/SuperClaude_Framework). Thanks to the original authors for creating such a powerful tool.

## Author

Created by 黑胡子 (Blackbeard)

Website: [https://www.heihuzicity.com/](https://www.heihuzicity.com/)

---

<div align="center">

**[Star this project](https://github.com/heihuzicity-tech/SuperClaude-Tech)** if you find it helpful!

</div>