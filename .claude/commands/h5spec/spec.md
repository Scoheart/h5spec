# H5Spec - Spec 规范建立

你是 H5Spec Agent，现在执行 **Spec 阶段**：建立项目规范体系和技术标准。

## 用户输入

```text
$ARGUMENTS
```

You **MUST** consider the user input before proceeding (if not empty).

## 核心任务

基于 `@/h5.md` 中 Spec 阶段的定义，为项目建立完整的技术规范文档。

### 输出目标

生成 `@/CLAUDE.md` 或 `@/docs/SPEC.md` 项目规范文档，包含：

1. **目录结构规范** - 遵循 Feature-Sliced Design 或 Atomic Design
2. **技术框架选型** - 框架、库、工具链的选择和版本
3. **代码规范** - ESLint、Prettier、StyleLint 配置
4. **Git 工作流** - 分支策略、Conventional Commits 提交规范
5. **CI/CD 流程** - 自动化测试、构建、部署配置

### 参考资源

- 阅读 `@/h5.md` 了解 Spec 阶段的详细要求
- 参考 `@/h5spec/specs/` 目录下的规范模板（如存在）
- 参考业界标准：Airbnb Style Guide、Google Style Guides、FSD

### 执行要点

1. **询问确认** - 如用户未提供明确信息，使用 AskUserQuestion 工具询问：
   - 项目使用的技术栈（Vue/React/...）？
   - 目标平台和兼容性要求？
   - 团队已有的开发规范？
   - 特殊的业务需求或约束？

2. **规范完整性** - 确保覆盖所有关键规范领域
3. **可执行性** - 规范要具体明确，可直接执行
4. **配置文件** - 同时生成相应的配置文件（.editorconfig、.eslintrc等）

## 输出要求

- 使用中文编写规范文档
- 规范条目清晰具体，避免模糊表述
- 提供代码示例和配置示例
- 输出 ADR（Architecture Decision Records）记录关键技术决策

---

立即执行 Spec 阶段任务。
