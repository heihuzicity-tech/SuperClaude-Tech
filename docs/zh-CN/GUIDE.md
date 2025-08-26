# SuperClaude v4 使用指南

## 📚 目录
- [核心功能](#核心功能)
- [常用示例](#常用示例)
- [高级功能](#高级功能)
- [使用技巧](#使用技巧)
- [快速参考](#快速参考)

## 🚀 核心功能

### 1. 斜杠命令 (v4格式：/sc:命令)
SuperClaude v4使用统一的 `/sc:` 命名空间，共21个命令。

#### 核心开发命令（8个必备）
| 命令 | 用途 | 示例 |
|------|------|------|
| `/sc:analyze` | 代码分析、审查、评估 | `/sc:analyze "分析代码性能问题"` |
| `/sc:troubleshoot` | 故障排查、调试、问题修复 | `/sc:troubleshoot "调试WebSocket连接问题"` |
| `/sc:implement` | 实现功能、开发、创建 | `/sc:implement "实现用户认证功能"` |
| `/sc:improve` | 优化、改进、提升 | `/sc:improve "优化数据库查询性能"` |
| `/sc:test` | 测试、验证、检验 | `/sc:test "为登录功能编写测试"` |
| `/sc:document` | 生成文档、说明、指南 | `/sc:document "为API生成文档"` |
| `/sc:brainstorm` | 项目发现、需求探索 | `/sc:brainstorm "探索项目需求"` |
| `/sc:workflow` | 实施规划、流程设计 | `/sc:workflow "制定开发计划"` |

#### 扩展命令（13个）
| 命令 | 用途 | 示例 |
|------|------|------|
| `/sc:build` | 构建完整功能或系统 | `/sc:build "构建用户管理系统"` |
| `/sc:design` | 系统设计、架构规划 | `/sc:design "设计微服务架构"` |
| `/sc:explain` | 解释代码、概念、原理 | `/sc:explain "解释算法工作原理"` |
| `/sc:estimate` | 工作估算、时间评估 | `/sc:estimate "估算项目时间"` |
| `/sc:git` | Git操作、版本控制 | `/sc:git "创建分支并提交"` |
| `/sc:cleanup` | 代码清理、删除无用代码 | `/sc:cleanup "清理技术债务"` |
| `/sc:reflect` | 反思总结、项目回顾 | `/sc:reflect "项目总结"` |
| `/sc:save` | 保存状态、持久化会话 | `/sc:save "保存当前进度"` |
| `/sc:load` | 加载状态、恢复会话 | `/sc:load "恢复之前的工作"` |
| `/sc:index` | 项目索引、结构分析 | `/sc:index "创建项目索引"` |
| `/sc:select-tool` | 工具选择、智能推荐 | `/sc:select-tool "推荐最佳工具"` |
| `/sc:spawn` | 创建实例、生成组件 | `/sc:spawn "生成新组件"` |
| `/sc:task` | 任务管理、分解跟踪 | `/sc:task "管理项目任务"` |

### 2. AI代理系统 (v4格式：@agent-名称)
SuperClaude v4提供14个专业AI代理，覆盖架构、开发、质量、分析等领域。

#### 架构与系统设计（3个）
| AI代理 | 专业领域 | 使用场景 |
|---------|----------|----------|
| `@agent-system-architect` | 🏢 大规模分布式系统 | 系统设计、架构规划、技术选型 |
| `@agent-frontend-architect` | 🎨 前端架构与UI/UX | 界面开发、用户体验、响应式设计 |
| `@agent-backend-architect` | ⚙️ 后端架构与服务 | 服务端开发、API设计、数据库优化 |

#### 开发与实现（3个）
| AI代理 | 专业领域 | 使用场景 |
|---------|----------|----------|
| `@agent-python-expert` | 🐍 Python开发专家 | Python开发、框架应用、最佳实践 |
| `@agent-devops-architect` | 🚀 DevOps与基础设施 | CI/CD、部署自动化、监控告警 |
| `@agent-refactoring-expert` | 🔧 代码重构专家 | 代码质量、技术债务、重构方案 |

#### 质量与安全（3个）
| AI代理 | 专业领域 | 使用场景 |
|---------|----------|----------|
| `@agent-security-engineer` | 🛡️ 安全工程师 | 安全审计、漏洞分析、威胁建模 |
| `@agent-quality-engineer` | 🧪 质量保证工程师 | 测试策略、质量控制、自动化测试 |
| `@agent-performance-engineer` | ⚡ 性能优化工程师 | 性能分析、瓶颈定位、优化方案 |

#### 分析与支持（5个）
| AI代理 | 专业领域 | 使用场景 |
|---------|----------|----------|
| `@agent-root-cause-analyst` | 🔍 根因分析专家 | 问题诊断、故障排查、系统调试 |
| `@agent-requirements-analyst` | 📋 需求分析师 | 需求分析、规格设计、用户故事 |
| `@agent-technical-writer` | ✍️ 技术文档专家 | 技术文档、API文档、用户手册 |
| `@agent-socratic-mentor` | 👨‍🏫 苏格拉底式导师 | 知识传授、引导式学习、技术指导 |
| `@agent-learning-guide` | 📚 学习指导专家 | 学习路径、概念解释、实践指导 |

### 3. 思考深度控制
根据问题复杂度选择合适的分析深度。

| 标志 | Token预算 | 使用场景 |
|------|-----------|----------|
| `--think` | 4K tokens | 模块级分析、常规问题 |
| `--think-hard` | 10K tokens | 系统级分析、复杂问题 |
| `--ultrathink` | 32K tokens | 企业级分析、全面审查（v4.0.8标准） |

### 4. MCP服务器（6个）
利用专门的MCP服务器扩展Claude的能力。

| 服务器 | 功能 | 使用标志 |
|--------|------|----------|
| `context7` | 📚 官方文档、代码示例、最佳实践 | `--c7` |
| `sequential-thinking` | 🧠 复杂分析、系统调试、架构审查 | `--seq` |
| `magic` | ✨ UI组件生成、设计系统集成 | `--magic` |
| `playwright` | 🎭 端到端测试、自动化、性能监控 | `--play` |
| `morphllm-fast-apply` | 🔄 代码转换、重构、迁移 | `--morph` |
| `serena` | 🧠 语义理解、项目记忆、上下文管理 | `--serena` |

## 🎯 智能指令转换模式

### 极简暗号激活（v4新功能）
```yaml
sc = SuperClaude转换模式（只转换指令）
无sc = 正常Claude对话模式（可执行任务）
```

### 使用示例
```bash
# 带sc暗号 - 转换模式
sc 优化数据库
→ 输出：/sc:improve "数据库优化" @agent-performance-engineer ...

# 不带sc - 正常模式  
优化这段代码
→ 直接执行优化任务
```

## 📋 常用示例

### 故障排查
```bash
# 调试登录问题
/sc:troubleshoot "用户登录后session丢失" @agent-backend-architect --think-hard

# 分析性能瓶颈
/sc:troubleshoot "页面加载超过5秒" @agent-performance-engineer --seq --think-hard

# WebSocket连接问题
/sc:troubleshoot "WebSocket连接频繁断开" @agent-backend-architect @agent-root-cause-analyst --trace
```

### 功能实现
```bash
# 实现暗黑模式
/sc:implement "添加暗黑模式切换功能" @agent-frontend-architect --with-tests

# 开发认证系统
/sc:implement "JWT认证系统" @agent-backend-architect @agent-security-engineer --safe-mode

# 创建响应式布局
/sc:implement "响应式导航栏" @agent-frontend-architect --magic
```

### 性能优化
```bash
# 优化首页加载
/sc:improve "优化首页加载速度" @agent-performance-engineer --systematic

# 数据库查询优化
/sc:improve "优化复杂查询性能" @agent-backend-architect @agent-performance-engineer --think-hard

# 前端渲染优化
/sc:improve "React组件渲染性能" @agent-frontend-architect @agent-performance-engineer --magic
```

### 安全审计
```bash
# 审查认证流程
/sc:analyze "审查用户认证流程" @agent-security-engineer --think-hard --safe-mode

# 漏洞扫描
/sc:analyze "检查SQL注入漏洞" @agent-security-engineer @agent-backend-architect --systematic

# 安全加固
/sc:improve "加强API安全性" @agent-security-engineer --with-tests --validate
```

### 代码分析
```bash
# 架构评审
/sc:analyze "评审微服务架构" @agent-system-architect --think-hard

# 代码质量检查
/sc:analyze "检查代码质量和技术债务" @agent-refactoring-expert --systematic

# 依赖分析
/sc:analyze "分析项目依赖关系" @agent-system-architect @agent-root-cause-analyst
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
/sc:build "构建完整的电商系统" --wave-mode auto --wave-strategy systematic

# 企业级重构
/sc:improve "重构遗留系统" --wave-mode force --wave-strategy enterprise

# 全面优化
/sc:improve "全面优化系统性能" --wave-mode auto --wave-strategy progressive
```

### 执行控制标志

| 标志 | 功能 | 使用场景 |
|------|------|----------|
| `--safe-mode` | 生产环境安全模式 | 关键系统、生产环境 |
| `--with-tests` | 包含测试代码 | 质量保证、TDD开发 |
| `--systematic` | 系统化执行 | 全面分析、深入检查 |
| `--validate` | 包含验证步骤 | 风险评估、质量检查 |
| `--trace` | 详细跟踪信息 | 调试、问题定位 |
| `--preview` | 预览模式，不执行 | 查看更改、评估影响 |
| `--focus [area]` | 聚焦特定领域 | 专项优化、定向分析 |

### 输出控制标志

| 标志 | 功能 | 使用场景 |
|------|------|----------|
| `--verbose` | 详细输出 | 深入了解执行过程 |
| `--quiet` | 最小输出 | 简洁结果展示 |
| `--format [md/json/yaml]` | 输出格式 | 特定格式需求 |
| `--uc` | 超压缩模式 | Token节省、快速响应 |
| `--interactive` | 交互式模式 | 逐步确认、协作探索 |

## 💡 使用技巧

### 1. 组合使用
可以组合多个代理和标志以获得最佳效果：

```bash
# 前后端联合分析
/sc:analyze "分析全栈应用性能" @agent-frontend-architect @agent-backend-architect @agent-performance-engineer --think-hard

# 安全性能平衡
/sc:improve "优化加密算法" @agent-security-engineer @agent-performance-engineer --ultrathink
```

### 2. 智能转换示例

#### 实际测试示例

- **输入**: `sc 网站访问很慢`
- **转换**: `/sc:troubleshoot "网站访问性能问题" @agent-performance-engineer @agent-frontend-architect @agent-root-cause-analyst --seq --play --ultrathink`

- **输入**: `sc 做个登录系统`
- **转换**: `/sc:implement "JWT用户认证系统" @agent-security-engineer @agent-backend-architect --c7 --safe-mode --with-tests --validate`

- **输入**: `sc 修复这个bug`
- **转换**: `/sc:troubleshoot "bug诊断与修复" @agent-root-cause-analyst --seq --verbose --think-hard`

- **输入**: `sc 创建REST API`
- **转换**: `/sc:implement "RESTful API服务" @agent-backend-architect --c7 --with-tests`

- **输入**: `sc 分析代码质量`
- **转换**: `/sc:analyze . @agent-quality-engineer @agent-refactoring-expert --seq --ultrathink --focus quality --systematic`

### 3. 任务复杂度评估
根据任务特征选择合适的配置：

| 复杂度 | 特征 | 推荐配置 |
|--------|------|----------|
| 简单 (0.0-0.4) | 单文件、直接任务 | 基础命令 + 单个代理 |
| 中等 (0.4-0.7) | 多文件、需要分析 | `--think` + 2-3个代理 |
| 复杂 (0.7-1.0) | 系统级、架构决策 | `--ultrathink` + Wave模式 + 多代理 |

### 4. 领域特定组合

#### 前端开发
```bash
/sc:implement "响应式组件" @agent-frontend-architect --magic --with-tests
/sc:improve "渲染性能" @agent-frontend-architect @agent-performance-engineer --play
```

#### 后端开发
```bash
/sc:implement "RESTful API" @agent-backend-architect --c7 --with-tests
/sc:troubleshoot "数据库死锁" @agent-backend-architect @agent-root-cause-analyst --seq
```

#### 全栈开发
```bash
/sc:build "用户管理系统" @agent-frontend-architect @agent-backend-architect --wave-mode auto
/sc:analyze "全栈性能" @agent-performance-engineer --seq --ultrathink
```

#### DevOps
```bash
/sc:implement "CI/CD流水线" @agent-devops-architect --systematic
/sc:improve "部署流程" @agent-devops-architect @agent-security-engineer --safe-mode
```

## 📝 快速参考

### 命令速查表
```bash
# 分析类
/sc:analyze "代码审查"
/sc:troubleshoot "问题诊断"
/sc:explain "概念解释"

# 开发类
/sc:implement "功能实现"
/sc:build "系统构建"
/sc:design "架构设计"

# 优化类
/sc:improve "性能优化"
/sc:cleanup "技术债务清理"

# 质量类
/sc:test "测试编写"
/sc:document "文档生成"

# 管理类
/sc:workflow "流程规划"
/sc:estimate "时间估算"
/sc:task "任务管理"

# 会话类
/sc:save "保存进度"
/sc:load "恢复进度"
```

### 常用组合
```bash
# 快速调试
/sc:troubleshoot "问题描述" --think

# 标准开发
/sc:implement "功能描述" --with-tests

# 深度分析
/sc:analyze "分析目标" --ultrathink --systematic

# 安全开发
/sc:implement "安全功能" @agent-security-engineer --safe-mode --validate

# 性能调优
/sc:improve "优化目标" @agent-performance-engineer --think-hard

# 企业级任务
/sc:build "大型系统" --wave-mode force --wave-strategy enterprise
```

### 官方推荐标志组合

#### 质量保证套件
```bash
/sc:implement "支付系统" @agent-security-engineer --safe-mode --with-tests --validate
```

#### 深度分析套件
```bash
/sc:troubleshoot "系统崩溃" @agent-root-cause-analyst --seq --ultrathink --systematic
```

#### 调试诊断套件
```bash
/sc:troubleshoot "内存泄漏" @agent-performance-engineer --trace --verbose --think-hard
```

#### 生产部署套件
```bash
/sc:build "生产版本" @agent-devops-architect --safe-mode --validate --preview
```

#### 性能优化套件
```bash
/sc:improve "API响应速度" @agent-performance-engineer --focus performance --systematic --with-tests
```

#### 安全审计套件
```bash
/sc:analyze . @agent-security-engineer --focus security --safe-mode --systematic --validate
```

#### 重构优化套件
```bash
/sc:improve . @agent-refactoring-expert --focus maintainability --with-tests --preview
```

## 🔄 常用工作流程

### 新项目启动（完整流程）
```bash
# 1. 需求探索与规划
/sc:brainstorm "项目概念" @agent-requirements-analyst --interactive
/sc:estimate "项目规模" @agent-system-architect --think-hard

# 2. 架构设计与验证
/sc:design "系统架构" @agent-system-architect @agent-devops-architect --seq --c7 --ultrathink
/sc:workflow "实施计划" @agent-system-architect --systematic

# 3. 核心功能实现
/sc:implement "核心功能" @agent-backend-architect @agent-frontend-architect --c7 --magic --with-tests --validate

# 4. 质量保证
/sc:test --coverage --systematic
/sc:analyze . --focus quality --safe-mode

# 5. 保存项目状态
/sc:save "项目初始版本"
```

### 问题诊断流程（生产环境）
```bash
# 1. 紧急诊断
/sc:troubleshoot "问题描述" @agent-root-cause-analyst --trace --verbose --safe-mode

# 2. 深入分析（并行执行）
/sc:analyze --focus performance @agent-performance-engineer --seq --systematic
/sc:analyze --focus security @agent-security-engineer --validate

# 3. 修复实施
/sc:improve --type performance @agent-performance-engineer --preview --safe-mode

# 4. 验证与部署
/sc:test --coverage --validate
/sc:build "修复版本" @agent-devops-architect --safe-mode --validate
```

### 代码优化流程（技术债务清理）
```bash
# 1. 全面分析
/sc:analyze . @agent-quality-engineer @agent-refactoring-expert --focus quality --systematic --trace

# 2. 制定重构计划
/sc:workflow "重构计划" @agent-refactoring-expert --think-hard

# 3. 分阶段优化
/sc:improve . @agent-refactoring-expert --focus maintainability --with-tests --preview
/sc:save "重构检查点"  # 保存进度

# 4. 验证改进
/sc:test --coverage --systematic
/sc:analyze . --focus quality  # 对比优化前后
```

## 🛠️ 调试模式系统

### 调试暗号激活
- 使用 `debug` 前缀可以进入调试模式，分析转换逻辑而不执行实际任务
- 示例：`debug 分析系统架构问题`

## 🔗 更多资源

- **完整文档**: 查看项目根目录的 `CLAUDE.md`
- **获取帮助**: 输入 `/help`
- **报告问题**: https://github.com/anthropics/claude-code/issues
- **SuperClaude项目**: 查看本地安装目录获取最新更新

## 📌 注意事项

1. **Token使用**: `--ultrathink` 会消耗大量token，谨慎使用
2. **生产环境**: 涉及生产系统时始终使用 `--safe-mode` 标志
3. **测试覆盖**: 关键功能建议使用 `--with-tests` 确保质量
4. **Wave模式**: 大型任务会自动激活，也可手动强制 `--wave-mode force`
5. **MCP服务器**: 某些MCP服务器（如magic、morphllm）可能需要API密钥配置

---

*SuperClaude v4.0.8 - 智能对话增强框架*
*最后更新：2025-08-26*