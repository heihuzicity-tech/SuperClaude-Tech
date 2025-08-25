# 📚 SuperClaude User Guide

## 🎯 What is SuperClaude-Tech?

SuperClaude-Tech is an intelligent instruction translation system that converts natural language into precise SuperClaude Framework commands. It helps you leverage the full power of Claude Code without memorizing complex command syntax.

## 🚀 Installation

### Method 1: Global Configuration
Place the `CLAUDE.md` file content in your global Claude Code configuration:
```
~/.claude/CLAUDE.md
```

### Method 2: Project Configuration
Place the `CLAUDE.md` file in your project root:
```
/your-project/CLAUDE.md
```

## 💡 Core Concept: The "sc" Activation Code

The system has two modes, controlled by a simple activation code:

| Mode | Activation | Function |
|------|-----------|----------|
| **Translation Mode** | Include `sc` in your input | Generates SuperClaude instructions |
| **Execution Mode** | No `sc` in your input | Claude executes tasks directly |

### Examples

**Translation Mode (with sc):**
```
Input: sc optimize my database queries
Output: /sc:improve "database query optimization" @agent-backend-architect --seq --think-hard
```

**Execution Mode (without sc):**
```
Input: optimize my database queries
Output: [Claude directly optimizes your code]
```

## 📋 Command Reference

### Core Development Commands

| Command | Purpose | Example |
|---------|---------|---------|
| `/sc:implement` | Create new features | `sc build a login form` |
| `/sc:analyze` | Analyze code quality | `sc check my code quality` |
| `/sc:troubleshoot` | Debug problems | `sc my app crashes` |
| `/sc:improve` | Optimize code | `sc make this faster` |
| `/sc:test` | Create tests | `sc write unit tests` |
| `/sc:document` | Generate docs | `sc document this API` |

### AI Agents

| Agent | Specialization | Auto-triggers |
|-------|---------------|---------------|
| `@agent-security-engineer` | Security & authentication | JWT, auth, encryption |
| `@agent-performance-engineer` | Performance optimization | slow, optimize, bottleneck |
| `@agent-frontend-architect` | UI/UX & frontend | React, component, responsive |
| `@agent-backend-architect` | Backend & APIs | API, database, server |
| `@agent-root-cause-analyst` | Debug & troubleshooting | error, bug, crash |

### MCP Servers

| Server | Purpose | Flag |
|--------|---------|------|
| Context7 | Official documentation | `--c7` |
| Sequential | Complex analysis | `--seq` |
| Magic | UI components | `--magic` |
| Playwright | Browser testing | `--play` |

### Thinking Depth Flags

| Flag | Token Usage | Use Case |
|------|------------|----------|
| `--think` | 4K tokens | Basic analysis |
| `--think-hard` | 10K tokens | Deep analysis |
| `--think-deep` | 32K tokens | Comprehensive analysis |

## 🎯 Common Use Cases

### 1. Performance Optimization
```bash
sc my website is slow
→ /sc:troubleshoot "website performance issues" @agent-performance-engineer --seq --think-hard
```

### 2. Security Implementation
```bash
sc add user authentication
→ /sc:implement "user authentication system" @agent-security-engineer --c7 --safe-mode
```

### 3. UI Development
```bash
sc create responsive navbar
→ /sc:implement "responsive navigation component" @agent-frontend-architect --magic
```

### 4. Bug Fixing
```bash
sc debug WebSocket connection
→ /sc:troubleshoot "WebSocket connection issues" @agent-root-cause-analyst --verbose
```

### 5. Code Review
```bash
sc review my code quality
→ /sc:analyze . @agent-quality-engineer --focus quality --think-hard
```

## 🔄 Workflows

### New Feature Development
1. `sc brainstorm user dashboard` - Explore requirements
2. `sc design dashboard architecture` - Plan structure
3. `sc implement dashboard` - Build feature
4. `sc test dashboard` - Validate functionality

### Problem Solving
1. `sc troubleshoot performance` - Diagnose issue
2. `sc analyze bottlenecks` - Deep analysis
3. `sc improve performance` - Apply fixes
4. `sc test improvements` - Verify solution

## 💡 Pro Tips

### 1. Combine Multiple Agents
```bash
sc build secure payment system
→ Multiple agents: @agent-security-engineer @agent-backend-architect
```

### 2. Use Appropriate Thinking Depth
- Simple tasks: No flag needed
- Complex debugging: `--think-hard`
- Architecture design: `--think-deep`

### 3. Leverage MCP Servers
- Documentation lookups: `--c7`
- Complex reasoning: `--seq`
- UI components: `--magic`

### 4. Focus Your Analysis
```bash
sc analyze security vulnerabilities
→ Adds: --focus security
```

## 🎯 Best Practices

### DO ✅
- Be specific in your descriptions
- Use `sc` only for instruction generation
- Combine agents for complex tasks
- Add appropriate flags for context

### DON'T ❌
- Don't use `sc` when you want immediate execution
- Don't overload with unnecessary flags
- Don't mix translation and execution modes

## 🔍 Troubleshooting

### Issue: Commands not generating properly
**Solution**: Ensure `sc` is at the beginning of your input

### Issue: Wrong agent selection
**Solution**: Be more specific with technical keywords

### Issue: Missing MCP servers
**Solution**: Explicitly mention the type of analysis needed

## 📈 Complexity Guidelines

### Simple Tasks (0.0-0.4)
- Single file operations
- Clear, direct requirements
- Use: 1 command + 1 agent

### Moderate Tasks (0.4-0.7)
- Multi-file operations
- Some analysis required
- Use: 1 command + 2-3 agents + `--think`

### Complex Tasks (0.7-1.0)
- System-level changes
- Architecture decisions
- Use: Multiple commands + agents + `--think-hard` + MCP

## 🚀 Quick Reference Card

```yaml
Activation: sc [your request]
Format: /sc:command "description" @agents --flags

Common Patterns:
  Performance: troubleshoot + @performance + --seq
  Security: implement + @security + --safe-mode
  UI: implement + @frontend + --magic
  Debug: troubleshoot + @root-cause + --verbose
  Analysis: analyze + @quality + --think-hard
```

## 📝 Examples Gallery

### Full-Stack Application
```bash
sc build todo app with React and Node.js
→ /sc:build "full-stack todo application" @agent-frontend-architect @agent-backend-architect --c7 --think-hard
```

### API Development
```bash
sc create REST API for products
→ /sc:implement "RESTful product API" @agent-backend-architect --c7 --with-tests
```

### Database Optimization
```bash
sc optimize slow queries
→ /sc:improve "database query performance" @agent-performance-engineer --seq --focus performance
```

### Security Audit
```bash
sc check security vulnerabilities
→ /sc:analyze . @agent-security-engineer --think-hard --focus security
```

## 🎓 Learning Path

1. **Start Simple**: Use basic commands without flags
2. **Add Agents**: Include relevant AI agents
3. **Use Flags**: Add thinking depth and MCP servers
4. **Combine**: Create complex multi-agent commands
5. **Master**: Understand when to use each combination

---

*Remember: `sc` for translation, no `sc` for execution!*