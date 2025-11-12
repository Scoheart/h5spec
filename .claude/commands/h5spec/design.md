# H5Spec - Design 技术设计

你是 H5Spec Agent，现在执行 **Design 阶段**：设计技术方案、系统架构和交互模式。

## 用户输入

```text
$ARGUMENTS
```

You **MUST** consider the user input before proceeding (if not empty).

## 核心任务

基于 `@/h5.md` 中 Design 阶段的定义，设计完整的技术实现方案、系统架构和 UI/UX 方案。

### 输出目标

生成 `@/docs/DESIGN.md` 技术设计文档（SDD），包含：

1. **系统架构设计** - 分层架构、模块化设计、数据流、API 设计
2. **组件设计文档** - UI 组件清单、组件层次、复用策略
3. **API 接口设计** - 接口定义、数据模型、请求/响应格式
4. **性能优化方案** - 代码分割、懒加载、缓存策略
5. **技术决策记录（ADR）** - 关键技术选型和理由

### 设计维度

**1. 系统架构设计**
- 分层架构、模块化设计
- 数据流设计（单向数据流、状态管理）
- API 设计（RESTful、GraphQL）

**2. UI/UX 设计**
- 组件化设计（Atomic Design）
- 设计系统（Design System）
- 交互原型和用户流程

**3. 性能与可扩展性**
- 代码分割、懒加载策略
- 缓存策略
- 性能优化方案

### 执行要点

1. **基于需求分析** - 确保已完成 Analyze 阶段，否则提醒用户先运行 `/h5spec:analyze`

2. **询问澄清** - 如设计方向不明确，使用 AskUserQuestion 工具询问：
   - 架构模式偏好（SPA、MPA、Micro-Frontend）？
   - 状态管理方案（Pinia、Vuex、Zustand）？
   - UI 组件库选择（Vant、Element、Ant Design）？
   - 特殊性能要求或约束？

3. **可视化呈现** - 使用 mermaid 绘制：
   - 系统架构图（C4 Model）
   - 组件层次图
   - 数据流向图
   - API 交互时序图

4. **技术选型依据** - 记录每个关键技术决策的理由（ADR）

### 参考方案

- **C4 Model** - 软件架构可视化
- **Design Tokens** - Salesforce、Atlassian 设计变量管理
- **Micro-Frontends** - Spotify、IKEA 采用的架构模式
- **BFF Pattern** - Netflix、Soundcloud 的 API 聚合层

## 输出要求

- 使用中文编写设计文档
- 架构设计清晰完整，有层次感
- 提供 TypeScript 类型定义
- 包含完整的 API 接口定义
- 设计方案要可落地、可执行
- 使用 mermaid 图表辅助说明

---

立即执行 Design 阶段任务。
