# SuperClaude 使用指南

## 📚 目录
- [核心功能](#核心功能)
- [常用示例](#常用示例)
- [高级功能](#高级功能)
- [使用技巧](#使用技巧)
- [快速参考](#快速参考)

## 🚀 核心功能

### 1. 斜杠命令 (Slash Commands)
在对话中直接使用斜杠命令来执行特定任务。

#### 基础命令
| 命令 | 用途 | 示例 |
|------|------|------|
| `/analyze` | 代码分析、审查、评估 | `/analyze "分析这段代码的性能问题"` |
| `/troubleshoot` | 故障排查、调试、问题修复 | `/troubleshoot "调试WebSocket连接问题"` |
| `/implement` | 实现功能、开发、创建 | `/implement "实现用户认证功能"` |
| `/improve` | 优化、改进、提升 | `/improve "优化数据库查询性能"` |
| `/test` | 测试、验证、检验 | `/test "为登录功能编写测试"` |
| `/document` | 生成文档、说明、指南 | `/document "为API生成文档"` |
| `/build` | 构建完整功能或系统 | `/build "构建用户管理系统"` |
| `/design` | 系统设计、架构规划 | `/design "设计微服务架构"` |
| `/explain` | 解释代码、概念、原理 | `/explain "解释这个算法的工作原理"` |

### 2. 专业角色 (Personas)
激活不同的专业AI角色来获得领域专家级的帮助。

#### 11个专业Personas
| Persona | 专业领域 | 使用场景 |
|---------|----------|----------|
| `@agent-system-architect` | 🏗️ 系统架构专家 | 系统设计、架构规划、技术选型 |
| `@agent-frontend-architect` | 🎨 前端UI/UX专家 | 界面开发、用户体验、响应式设计 |
| `@agent-backend-architect` | ⚙️ 后端工程师 | 服务端开发、API设计、数据库优化 |
| `@agent-security-engineer` | 🛡️ 安全专家 | 安全审计、漏洞分析、威胁建模 |
| `@agent-performance-engineer` | ⚡ 性能优化专家 | 性能分析、瓶颈定位、优化方案 |
| `@agent-root-cause-analyst` | 🔍 根因分析专家 | 问题诊断、故障排查、系统调试 |
| `@agent-quality-engineer` | 🧪 质量保证专家 | 测试策略、质量控制、自动化测试 |
| `@agent-devops-architect` | 🚀 DevOps专家 | CI/CD、部署自动化、监控告警 |
| `@agent-refactoring-expert` | 🔧 代码重构专家 | 代码质量、技术债务、重构方案 |
| `@agent-socratic-mentor` | 👨‍🏫 技术导师 | 知识传授、最佳实践、技术指导 |
| `@agent-technical-writer` | ✍️ 文档专家 | 技术文档、API文档、用户手册 |

### 3. 思考深度控制
根据问题复杂度选择合适的分析深度。

| 标志 | Token预算 | 使用场景 |
|------|-----------|----------|
| `--think` | 4K tokens | 模块级分析、常规问题 |
| `--think-hard` | 10K tokens | 系统级分析、复杂问题 |
| `--ultrathink` | 32K tokens | 企业级分析、关键系统 |

### 4. MCP服务器
利用专门的MCP服务器扩展Claude的能力。

| 服务器 | 功能 | 使用标志 |
|--------|------|----------|
| Context7 | 📚 官方文档、代码示例、最佳实践 | `--c7` |
| Sequential | 🧠 复杂分析、系统调试、架构审查 | `--seq` |
| Magic | ✨ UI组件生成、设计系统集成 | `--magic` |
| Playwright | 🎭 端到端测试、自动化、性能监控 | `--play` |
| 全部启用 | 启用所有MCP服务器 | `--all-mcp` |
| 全部禁用 | 禁用所有MCP服务器 | `--no-mcp` |

## 📋 常用示例

### 故障排查
```bash
# 调试登录问题
/troubleshoot "用户登录后session丢失" @agent-backend-architect --think-hard

# 分析性能瓶颈
/troubleshoot "页面加载超过5秒" @agent-performance-engineer --seq --think-hard

# WebSocket连接问题
/troubleshoot "WebSocket连接频繁断开" @agent-backend-architect @agent-root-cause-analyst --trace
```

### 功能实现
```bash
# 实现暗黑模式
/implement "添加暗黑模式切换功能" @agent-frontend-architect --with-tests

# 开发认证系统
/implement "JWT认证系统" @agent-backend-architect @agent-security-engineer --safe

# 创建响应式布局
/implement "响应式导航栏" @agent-frontend-architect --magic
```

### 性能优化
```bash
# 优化首页加载
/improve "优化首页加载速度" @agent-performance-engineer --systematic

# 数据库查询优化
/improve "优化复杂查询性能" @agent-backend-architect @agent-performance-engineer --think-hard

# 前端渲染优化
/improve "React组件渲染性能" @agent-frontend-architect @agent-performance-engineer --magic
```

### 安全审计
```bash
# 审查认证流程
/analyze "审查用户认证流程" @agent-security-engineer --think-hard --safe

# 漏洞扫描
/analyze "检查SQL注入漏洞" @agent-security-engineer @agent-backend-architect --systematic

# 安全加固
/improve "加强API安全性" @agent-security-engineer --with-tests --validate
```

### 代码分析
```bash
# 架构评审
/analyze "评审微服务架构" @agent-system-architect --think-hard

# 代码质量检查
/analyze "检查代码质量和技术债务" @agent-refactoring-expert --systematic

# 依赖分析
/analyze "分析项目依赖关系" @agent-system-architect @agent-root-cause-analyst
```

## 🌊 高级功能

### Wave模式（复杂任务编排）
Wave模式用于处理大型复杂任务，自动将任务分解为多个协调阶段。

#### 自动激活条件
- 任务复杂度 ≥ 0.7
- 涉及文件数 > 20
- 操作类型 > 2种

#### Wave策略
| 策略 | 适用场景 | 使用标志 |
|------|----------|----------|
| Progressive | 渐进式增强、逐步优化 | `--wave-strategy progressive` |
| Systematic | 系统化方法、全面分析 | `--wave-strategy systematic` |
| Adaptive | 自适应配置、动态调整 | `--wave-strategy adaptive` |
| Enterprise | 企业级编排、大规模项目 | `--wave-strategy enterprise` |

#### 示例
```bash
# 构建完整系统
/build "构建完整的电商系统" --wave-mode auto --wave-strategy systematic

# 企业级重构
/improve "重构遗留系统" --wave-mode force --wave-strategy enterprise

# 全面优化
/improve "全面优化系统性能" --wave-mode auto --wave-strategy progressive
```

### 执行控制标志

| 标志 | 功能 | 使用场景 |
|------|------|----------|
| `--safe` | 生产环境安全模式 | 关键系统、生产环境 |
| `--with-tests` | 包含测试代码 | 质量保证、TDD开发 |
| `--systematic` | 系统化执行 | 全面分析、深入检查 |
| `--validate` | 包含验证步骤 | 风险评估、质量检查 |
| `--trace` | 详细跟踪信息 | 调试、问题定位 |
| `--documentation` | 生成文档 | 项目文档、API说明 |

## 💡 使用技巧

### 1. 组合使用
可以组合多个persona和标志以获得最佳效果：

```bash
# 前后端联合分析
/analyze "分析全栈应用性能" @agent-frontend-architect @agent-backend-architect @agent-performance-engineer --think-hard

# 安全性能平衡
/improve "优化加密算法" @agent-security-engineer @agent-performance-engineer --ultrathink
```

### 2. 智能转换模式
使用自然语言描述，系统会自动转换为最优SuperClaude指令：

#### 实际测试示例

- **输入**: `sc 网站访问很慢`
- **转换**: `/sc:troubleshoot "网站访问性能问题诊断" @agent-performance-engineer @agent-frontend-architect @agent-root-cause-analyst --seq --play --think-hard`

- **输入**: `sc 做个登录系统`
- **转换**: `/sc:implement "用户登录认证系统" @agent-security-engineer @agent-backend-architect --c7 --safe-mode --with-tests`

- **输入**: `sc 修复这个bug`
- **转换**: `/sc:troubleshoot "bug诊断与修复" @agent-root-cause-analyst --seq --verbose`

- **输入**: `sc 创建REST API`
- **转换**: `/sc:implement "RESTful API服务" @agent-backend-architect --c7 --with-tests`

- **输入**: `sc 分析代码质量`
- **转换**: `/sc:analyze . @agent-quality-engineer @agent-refactoring-expert --seq --think-hard --focus quality`

### 3. 任务复杂度评估
根据任务特征选择合适的配置：

| 复杂度 | 特征 | 推荐配置 |
|--------|------|----------|
| 简单 (0.0-0.4) | 单文件、直接任务 | 基础命令 + 单个persona |
| 中等 (0.4-0.7) | 多文件、需要分析 | `--think` + 2个persona |
| 复杂 (0.7-1.0) | 系统级、架构决策 | `--think-hard` + Wave模式 |

### 4. 领域特定组合

#### 前端开发
```bash
/implement "响应式组件" @agent-frontend-architect --magic --with-tests
/improve "渲染性能" @agent-frontend-architect @agent-performance-engineer --play
```

#### 后端开发
```bash
/implement "RESTful API" @agent-backend-architect --c7 --with-tests
/troubleshoot "数据库死锁" @agent-backend-architect @agent-root-cause-analyst --seq
```

#### 全栈开发
```bash
/build "用户管理系统" @agent-frontend-architect @agent-backend-architect --wave-mode auto
/analyze "全栈性能" @agent-performance-engineer --all-mcp --think-hard
```

#### DevOps
```bash
/implement "CI/CD流水线" @agent-devops-architect --systematic
/improve "部署流程" @agent-devops-architect @agent-security-engineer --safe
```

## 📝 快速参考

### 命令速查表
```bash
# 分析类
/analyze "代码审查"
/troubleshoot "问题诊断"
/explain "概念解释"

# 开发类
/implement "功能实现"
/build "系统构建"
/design "架构设计"

# 优化类
/improve "性能优化"
/refactor "代码重构"

# 质量类
/test "测试编写"
/document "文档生成"
```

### 常用组合
```bash
# 快速调试
/troubleshoot "问题描述" --think

# 标准开发
/implement "功能描述" --with-tests

# 深度分析
/analyze "分析目标" --think-hard --systematic

# 安全开发
/implement "安全功能" @agent-security-engineer --safe --validate

# 性能调优
/improve "优化目标" @agent-performance-engineer --think-hard

# 企业级任务
/build "大型系统" --wave-mode force --wave-strategy enterprise
```

### 调试暗号
- 使用 `debug` 前缀可以进入调试模式，分析转换逻辑而不执行实际任务
- 示例：`debug 分析系统架构问题`

## 🔗 更多资源

- **完整文档**: `~/.claude` 目录
- **获取帮助**: 输入 `/help`
- **报告问题**: https://github.com/anthropics/claude-code/issues
- **SuperClaude项目**: 查看本地安装目录获取最新更新

## 📌 注意事项

1. **Token使用**: `--ultrathink` 会消耗大量token，谨慎使用
2. **生产环境**: 涉及生产系统时始终使用 `--safe` 标志
3. **测试覆盖**: 关键功能建议使用 `--with-tests` 确保质量
4. **Wave模式**: 大型任务会自动激活，也可手动强制 `--wave-mode force`
5. **MCP服务器**: 某些MCP服务器可能需要API密钥配置

---

*SuperClaude v4.0.8 - 智能对话增强框架*
*最后更新：2025-08-25*