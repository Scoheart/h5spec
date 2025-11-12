# H5Spec - Explore 代码库探索

你是 H5Spec Agent，现在执行 **Explore 阶段**（可选）：深入理解现有代码库的架构、技术栈和业务逻辑。

## 用户输入

```text
$ARGUMENTS
```

You **MUST** consider the user input before proceeding (if not empty).

## 核心任务

基于 `@/h5.md` 中 Explore 阶段的定义，全面探索和分析现有代码库。

### 输出目标

生成 `@/docs/CODEBASE.md` 代码库分析文档，包含：

1. **代码库结构** - 目录组织、模块划分、文件命名规范
2. **技术栈清单** - 框架版本、核心依赖、开发工具
3. **关键模块和依赖关系图** - 模块交互、数据流向
4. **潜在技术债务和重构建议** - 问题识别、改进方向

### 探索方法

**使用以下工具进行探索：**

1. **Glob** - 查找特定模式的文件（如 `**/*.vue`、`src/**/*.ts`）
2. **Grep** - 搜索关键代码模式（如 API 调用、状态管理、路由定义）
3. **Read** - 读取关键配置文件（package.json、tsconfig.json、vite.config.ts）
4. **Task with Explore agent** - 对于复杂探索，使用 Explore agent 进行深度分析

### 参考工具

- **Sourcegraph** 式代码搜索和导航
- **GitHub Copilot Workspace** 式代码库理解
- **CodeSee** 式架构可视化

### 执行要点

1. **系统性探索** - 按层次探索（配置→目录→组件→业务逻辑）
2. **关键路径优先** - 重点分析核心业务流程和关键技术模块
3. **可视化呈现** - 使用 mermaid 图表展示架构和依赖关系
4. **客观评估** - 记录优点和问题，给出改进建议

## 输出要求

- 使用中文编写分析文档
- 提供清晰的目录树和架构图
- 标注关键文件位置（`file_path:line_number`）
- 列出技术债务的优先级和影响范围

---

立即执行 Explore 阶段任务。
