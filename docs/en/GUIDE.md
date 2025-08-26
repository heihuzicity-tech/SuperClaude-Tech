# SuperClaude v4 User Guide

## 📚 Table of Contents
- [Core Features](#core-features)
- [Common Examples](#common-examples)
- [Advanced Features](#advanced-features)
- [Usage Tips](#usage-tips)
- [Quick Reference](#quick-reference)

## 🚀 Core Features

### 1. Slash Commands (v4 format: /sc:command)
SuperClaude v4 uses a unified `/sc:` namespace with 21 commands total.

#### Core Development Commands (8 essentials)
| Command | Purpose | Example |
|---------|---------|---------|
| `/sc:analyze` | Code analysis, review, evaluation | `/sc:analyze "analyze code performance issues"` |
| `/sc:troubleshoot` | Troubleshooting, debugging, problem fixing | `/sc:troubleshoot "debug WebSocket connection issues"` |
| `/sc:implement` | Implement features, develop, create | `/sc:implement "implement user authentication"` |
| `/sc:improve` | Optimize, enhance, improve | `/sc:improve "optimize database query performance"` |
| `/sc:test` | Test, validate, verify | `/sc:test "write tests for login feature"` |
| `/sc:document` | Generate documentation, guides | `/sc:document "generate API documentation"` |
| `/sc:brainstorm` | Project discovery, requirement exploration | `/sc:brainstorm "explore project requirements"` |
| `/sc:workflow` | Implementation planning, process design | `/sc:workflow "create development plan"` |

#### Extended Commands (13)
| Command | Purpose | Example |
|---------|---------|---------|
| `/sc:build` | Build complete feature or system | `/sc:build "build user management system"` |
| `/sc:design` | System design, architecture planning | `/sc:design "design microservices architecture"` |
| `/sc:explain` | Explain code, concepts, principles | `/sc:explain "explain algorithm logic"` |
| `/sc:estimate` | Work estimation, time assessment | `/sc:estimate "estimate project timeline"` |
| `/sc:git` | Git operations, version control | `/sc:git "create branch and commit"` |
| `/sc:cleanup` | Code cleanup, remove unused code | `/sc:cleanup "clean technical debt"` |
| `/sc:reflect` | Reflection summary, project review | `/sc:reflect "project retrospective"` |
| `/sc:save` | Save state, persist session | `/sc:save "save current progress"` |
| `/sc:load` | Load state, restore session | `/sc:load "restore previous work"` |
| `/sc:index` | Project index, structure analysis | `/sc:index "create project index"` |
| `/sc:select-tool` | Tool selection, intelligent recommendation | `/sc:select-tool "recommend best tools"` |
| `/sc:spawn` | Create instance, generate component | `/sc:spawn "generate new component"` |
| `/sc:task` | Task management, breakdown tracking | `/sc:task "manage project tasks"` |

### 2. AI Agent System (v4 format: @agent-name)
SuperClaude v4 provides 14 professional AI agents covering architecture, development, quality, and analysis domains.

#### Architecture & System Design (3)
| AI Agent | Specialization | Use Cases |
|----------|----------------|-----------|
| `@agent-system-architect` | 🏢 Large-scale distributed systems | System design, architecture planning, tech selection |
| `@agent-frontend-architect` | 🎨 Frontend architecture & UI/UX | Interface development, user experience, responsive design |
| `@agent-backend-architect` | ⚙️ Backend architecture & services | Server development, API design, database optimization |

#### Development & Implementation (3)
| AI Agent | Specialization | Use Cases |
|----------|----------------|-----------|
| `@agent-python-expert` | 🐍 Python development expert | Python development, framework usage, best practices |
| `@agent-devops-architect` | 🚀 DevOps & infrastructure | CI/CD, deployment automation, monitoring & alerts |
| `@agent-refactoring-expert` | 🔧 Code refactoring expert | Code quality, technical debt, refactoring solutions |

#### Quality & Security (3)
| AI Agent | Specialization | Use Cases |
|----------|----------------|-----------|
| `@agent-security-engineer` | 🛡️ Security engineer | Security audit, vulnerability analysis, threat modeling |
| `@agent-quality-engineer` | 🧪 Quality assurance engineer | Testing strategy, quality control, test automation |
| `@agent-performance-engineer` | ⚡ Performance optimization engineer | Performance analysis, bottleneck detection, optimization solutions |

#### Analysis & Support (5)
| AI Agent | Specialization | Use Cases |
|----------|----------------|-----------|
| `@agent-root-cause-analyst` | 🔍 Root cause analysis expert | Problem diagnosis, troubleshooting, system debugging |
| `@agent-requirements-analyst` | 📋 Requirements analyst | Requirements analysis, specification design, user stories |
| `@agent-technical-writer` | ✍️ Technical documentation expert | Technical docs, API documentation, user manuals |
| `@agent-socratic-mentor` | 👨‍🏫 Socratic mentor | Knowledge transfer, guided learning, technical mentoring |
| `@agent-learning-guide` | 📚 Learning guidance expert | Learning paths, concept explanation, practical guidance |

### 3. Thinking Depth Control
Choose appropriate analysis depth based on problem complexity.

| Flag | Token Budget | Use Case |
|------|-------------|----------|
| `--think` | 4K tokens | Module-level analysis, routine problems |
| `--think-hard` | 10K tokens | System-level analysis, complex problems |
| `--ultrathink` | 32K tokens | Enterprise-level analysis, comprehensive review (v4.0.8 standard) |

### 4. MCP Servers (6)
Leverage specialized MCP servers to extend Claude's capabilities.

| Server | Function | Flag |
|--------|----------|------|
| `context7` | 📚 Official docs, code examples, best practices | `--c7` |
| `sequential-thinking` | 🧠 Complex analysis, system debugging, architecture review | `--seq` |
| `magic` | ✨ UI component generation, design system integration | `--magic` |
| `playwright` | 🎭 End-to-end testing, automation, performance monitoring | `--play` |
| `morphllm-fast-apply` | 🔄 Code transformation, refactoring, migration | `--morph` |
| `serena` | 🧠 Semantic understanding, project memory, context management | `--serena` |

## 🎯 Intelligent Instruction Translation Mode

### Simple Activation Code (v4 new feature)
```yaml
sc = SuperClaude translation mode (only translates instructions)
no sc = Normal Claude conversation mode (can execute tasks)
```

### Usage Examples
```bash
# With sc code - Translation mode
sc optimize database
→ Output: /sc:improve "database optimization" @agent-performance-engineer ...

# Without sc - Normal mode  
optimize this code
→ Directly executes optimization task
```

## 📋 Common Examples

### Troubleshooting
```bash
# Debug login issues
/sc:troubleshoot "user session lost after login" @agent-backend-architect --think-hard

# Analyze performance bottlenecks
/sc:troubleshoot "page loads over 5 seconds" @agent-performance-engineer --seq --think-hard

# WebSocket connection issues
/sc:troubleshoot "WebSocket disconnects frequently" @agent-backend-architect @agent-root-cause-analyst --trace
```

### Feature Implementation
```bash
# Implement dark mode
/sc:implement "add dark mode toggle feature" @agent-frontend-architect --with-tests

# Develop authentication system
/sc:implement "JWT authentication system" @agent-backend-architect @agent-security-engineer --safe-mode

# Create responsive layout
/sc:implement "responsive navigation bar" @agent-frontend-architect --magic
```

### Performance Optimization
```bash
# Optimize homepage loading
/sc:improve "optimize homepage load speed" @agent-performance-engineer --systematic

# Database query optimization
/sc:improve "optimize complex query performance" @agent-backend-architect @agent-performance-engineer --think-hard

# Frontend rendering optimization
/sc:improve "React component rendering performance" @agent-frontend-architect @agent-performance-engineer --magic
```

### Security Audit
```bash
# Review authentication flow
/sc:analyze "review user authentication flow" @agent-security-engineer --think-hard --safe-mode

# Vulnerability scanning
/sc:analyze "check SQL injection vulnerabilities" @agent-security-engineer @agent-backend-architect --systematic

# Security hardening
/sc:improve "strengthen API security" @agent-security-engineer --with-tests --validate
```

### Code Analysis
```bash
# Architecture review
/sc:analyze "review microservices architecture" @agent-system-architect --think-hard

# Code quality check
/sc:analyze "check code quality and technical debt" @agent-refactoring-expert --systematic

# Dependency analysis
/sc:analyze "analyze project dependencies" @agent-system-architect @agent-root-cause-analyst
```

## 🌊 Advanced Features

### Wave Mode (Complex Task Orchestration)
Wave mode handles large complex tasks by automatically breaking them into coordinated phases.

#### Auto-activation Conditions
- Task complexity ≥ 0.7
- Files involved > 20
- Operation types > 2

#### Wave Strategies
| Strategy | Use Case | Flag |
|----------|----------|------|
| Progressive | Incremental enhancement, gradual optimization | `--wave-strategy progressive` |
| Systematic | Systematic approach, comprehensive analysis | `--wave-strategy systematic` |
| Adaptive | Adaptive configuration, dynamic adjustment | `--wave-strategy adaptive` |
| Enterprise | Enterprise orchestration, large-scale projects | `--wave-strategy enterprise` |

#### Examples
```bash
# Build complete system
/sc:build "build complete e-commerce system" --wave-mode auto --wave-strategy systematic

# Enterprise refactoring
/sc:improve "refactor legacy system" --wave-mode force --wave-strategy enterprise

# Comprehensive optimization
/sc:improve "comprehensive system performance optimization" --wave-mode auto --wave-strategy progressive
```

### Execution Control Flags

| Flag | Function | Use Case |
|------|----------|----------|
| `--safe-mode` | Production environment safety | Critical systems, production env |
| `--with-tests` | Include test code | Quality assurance, TDD development |
| `--systematic` | Systematic execution | Comprehensive analysis, deep inspection |
| `--validate` | Include validation steps | Risk assessment, quality checks |
| `--trace` | Detailed trace information | Debugging, problem location |
| `--preview` | Preview mode, don't execute | View changes, assess impact |
| `--focus [area]` | Focus on specific domain | Targeted optimization, directed analysis |

### Output Control Flags

| Flag | Function | Use Case |
|------|----------|----------|
| `--verbose` | Detailed output | Deep understanding of execution |
| `--quiet` | Minimal output | Concise result display |
| `--format [md/json/yaml]` | Output format | Specific format needs |
| `--uc` | Ultra-compressed mode | Token saving, fast response |
| `--interactive` | Interactive mode | Step-by-step confirmation, collaborative exploration |

## 💡 Usage Tips

### 1. Combine Multiple Elements
Combine multiple agents and flags for best results:

```bash
# Full-stack analysis
/sc:analyze "analyze full-stack app performance" @agent-frontend-architect @agent-backend-architect @agent-performance-engineer --think-hard

# Security-performance balance
/sc:improve "optimize encryption algorithm" @agent-security-engineer @agent-performance-engineer --ultrathink
```

### 2. Intelligent Translation Examples

#### Real Test Examples

- **Input**: `sc website is slow`
- **Translation**: `/sc:troubleshoot "website performance issues" @agent-performance-engineer @agent-frontend-architect @agent-root-cause-analyst --seq --play --ultrathink`

- **Input**: `sc build login system`
- **Translation**: `/sc:implement "JWT user authentication system" @agent-security-engineer @agent-backend-architect --c7 --safe-mode --with-tests --validate`

- **Input**: `sc fix this bug`
- **Translation**: `/sc:troubleshoot "bug diagnosis and fix" @agent-root-cause-analyst --seq --verbose --think-hard`

- **Input**: `sc create REST API`
- **Translation**: `/sc:implement "RESTful API service" @agent-backend-architect --c7 --with-tests`

- **Input**: `sc analyze code quality`
- **Translation**: `/sc:analyze . @agent-quality-engineer @agent-refactoring-expert --seq --ultrathink --focus quality --systematic`

### 3. Task Complexity Assessment
Choose appropriate configuration based on task characteristics:

| Complexity | Features | Recommended Config |
|------------|----------|-------------------|
| Simple (0.0-0.4) | Single file, direct task | Basic command + single agent |
| Moderate (0.4-0.7) | Multiple files, needs analysis | `--think` + 2-3 agents |
| Complex (0.7-1.0) | System-level, architecture decisions | `--ultrathink` + Wave mode + multiple agents |

### 4. Domain-specific Combinations

#### Frontend Development
```bash
/sc:implement "responsive component" @agent-frontend-architect --magic --with-tests
/sc:improve "rendering performance" @agent-frontend-architect @agent-performance-engineer --play
```

#### Backend Development
```bash
/sc:implement "RESTful API" @agent-backend-architect --c7 --with-tests
/sc:troubleshoot "database deadlock" @agent-backend-architect @agent-root-cause-analyst --seq
```

#### Full-stack Development
```bash
/sc:build "user management system" @agent-frontend-architect @agent-backend-architect --wave-mode auto
/sc:analyze "full-stack performance" @agent-performance-engineer --seq --ultrathink
```

#### DevOps
```bash
/sc:implement "CI/CD pipeline" @agent-devops-architect --systematic
/sc:improve "deployment process" @agent-devops-architect @agent-security-engineer --safe-mode
```

## 📝 Quick Reference

### Command Cheat Sheet
```bash
# Analysis
/sc:analyze "code review"
/sc:troubleshoot "problem diagnosis"
/sc:explain "concept explanation"

# Development
/sc:implement "feature implementation"
/sc:build "system build"
/sc:design "architecture design"

# Optimization
/sc:improve "performance optimization"
/sc:cleanup "technical debt cleanup"

# Quality
/sc:test "test writing"
/sc:document "documentation generation"

# Management
/sc:workflow "process planning"
/sc:estimate "time estimation"
/sc:task "task management"

# Session
/sc:save "save progress"
/sc:load "restore progress"
```

### Common Combinations
```bash
# Quick debugging
/sc:troubleshoot "problem description" --think

# Standard development
/sc:implement "feature description" --with-tests

# Deep analysis
/sc:analyze "analysis target" --ultrathink --systematic

# Secure development
/sc:implement "security feature" @agent-security-engineer --safe-mode --validate

# Performance tuning
/sc:improve "optimization target" @agent-performance-engineer --think-hard

# Enterprise tasks
/sc:build "large system" --wave-mode force --wave-strategy enterprise
```

### Official Recommended Flag Combinations

#### Quality Assurance Suite
```bash
/sc:implement "payment system" @agent-security-engineer --safe-mode --with-tests --validate
```

#### Deep Analysis Suite
```bash
/sc:troubleshoot "system crash" @agent-root-cause-analyst --seq --ultrathink --systematic
```

#### Debug Diagnostics Suite
```bash
/sc:troubleshoot "memory leak" @agent-performance-engineer --trace --verbose --think-hard
```

#### Production Deployment Suite
```bash
/sc:build "production version" @agent-devops-architect --safe-mode --validate --preview
```

#### Performance Optimization Suite
```bash
/sc:improve "API response speed" @agent-performance-engineer --focus performance --systematic --with-tests
```

#### Security Audit Suite
```bash
/sc:analyze . @agent-security-engineer --focus security --safe-mode --systematic --validate
```

#### Refactoring Optimization Suite
```bash
/sc:improve . @agent-refactoring-expert --focus maintainability --with-tests --preview
```

## 🔄 Common Workflows

### New Project Startup (Complete Process)
```bash
# 1. Requirement exploration and planning
/sc:brainstorm "project concept" @agent-requirements-analyst --interactive
/sc:estimate "project scale" @agent-system-architect --think-hard

# 2. Architecture design and validation
/sc:design "system architecture" @agent-system-architect @agent-devops-architect --seq --c7 --ultrathink
/sc:workflow "implementation plan" @agent-system-architect --systematic

# 3. Core feature implementation
/sc:implement "core features" @agent-backend-architect @agent-frontend-architect --c7 --magic --with-tests --validate

# 4. Quality assurance
/sc:test --coverage --systematic
/sc:analyze . --focus quality --safe-mode

# 5. Save project state
/sc:save "initial project version"
```

### Problem Diagnosis Flow (Production Environment)
```bash
# 1. Emergency diagnosis
/sc:troubleshoot "problem description" @agent-root-cause-analyst --trace --verbose --safe-mode

# 2. Deep analysis (parallel execution)
/sc:analyze --focus performance @agent-performance-engineer --seq --systematic
/sc:analyze --focus security @agent-security-engineer --validate

# 3. Fix implementation
/sc:improve --type performance @agent-performance-engineer --preview --safe-mode

# 4. Validation and deployment
/sc:test --coverage --validate
/sc:build "fix version" @agent-devops-architect --safe-mode --validate
```

### Code Optimization Flow (Technical Debt Cleanup)
```bash
# 1. Comprehensive analysis
/sc:analyze . @agent-quality-engineer @agent-refactoring-expert --focus quality --systematic --trace

# 2. Create refactoring plan
/sc:workflow "refactoring plan" @agent-refactoring-expert --think-hard

# 3. Phased optimization
/sc:improve . @agent-refactoring-expert --focus maintainability --with-tests --preview
/sc:save "refactoring checkpoint"  # Save progress

# 4. Verify improvements
/sc:test --coverage --systematic
/sc:analyze . --focus quality  # Compare before and after
```

## 🛠️ Debug Mode System

### Debug Code Activation
- Use `debug` prefix to enter debug mode, analyze translation logic without executing tasks
- Example: `debug analyze system architecture issues`

## 🔗 More Resources

- **Complete Documentation**: See `CLAUDE.md` in project root
- **Get Help**: Type `/help`
- **Report Issues**: https://github.com/anthropics/claude-code/issues
- **SuperClaude Project**: Check local installation directory for updates

## 📌 Important Notes

1. **Token Usage**: `--ultrathink` consumes significant tokens, use carefully
2. **Production Environment**: Always use `--safe-mode` flag for production systems
3. **Test Coverage**: Critical features should use `--with-tests` for quality assurance
4. **Wave Mode**: Automatically activates for large tasks, can force with `--wave-mode force`
5. **MCP Servers**: Some MCP servers (like magic, morphllm) may require API key configuration

---

*SuperClaude v4.0.8 - Intelligent Conversation Enhancement Framework*
*Last Updated: 2025-08-26*