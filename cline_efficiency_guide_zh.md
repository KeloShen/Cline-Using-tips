# Cline 使用tips介绍
介绍一些我在短期使用过程中觉得比较常用且实用的小功能
---

## 1. Plan and Act 模式
相关Youtube官方视频：[How to Use Plan & Act Modes in Cline](https://www.youtube.com/watch?v=b7o6URFPp64)

**Plan and Act 模式** 将开发过程分为两个阶段，旨在通过前期的充分规划来减少后期的修改，从而节省时间和 token。


### 功能介绍
- **Plan 模式**: 在此模式下，您可以与 Cline 深入交流，明确任务需求、探索不同方案、并制定详细的执行策略。Cline 在这个阶段会像一个项目经理，利用其搜索、文件读取和分析能力，为您规划出最佳路径。这个阶段通常会选用推理能力强、上下文窗口大的模型，因为规划阶段的成本相对较低。
- **Act 模式**: 当您对计划感到满意后，可以切换到 Act 模式。Cline 会严格执行在 Plan 模式中确定的策略和上下文。在这个阶段，您可以切换到更擅长编码的模型，从而结合两种模型的优点：一个用于策略规划，一个用于代码实现。

### 使用方法
1.  **进入 Plan 模式**: 开始一个新任务时，主动切换到 Plan 模式。
2.  **详细沟通**: 与 Cline 充分沟通您的需求，让它读取相关文件、搜索文档，并提出实施计划。
3.  **确认计划**: 在您确认 Cline 完全理解任务并制定了可靠的计划后。
4.  **切换到 Act 模式**: 切换到 Act 模式，并可以选择一个更适合编码的模型来执行计划。

---

## 2. Memory Bank
相关Youtube官方视频： [Ideal Setup for Cline](https://www.youtube.com/watch?v=UBqh6ud5LqY)

**Memory Bank** 是一种让 Cline 在同一个项目的不同任务间共享和记忆上下文的技术。它确保了 Cline 在处理新任务时，能够“记住”项目的历史、技术选型和总体方向。

### 功能介绍
- **跨任务记忆**: 解决了在开启新任务时，需要重复提供项目背景信息的问题。
- **保持一致性**: 确保 Cline 的输出与项目的既有规范和架构保持一致。
- **项目演进**: 帮助 Cline 理解项目的演进过程，从而提供更贴切的建议和代码。

### 使用方法
1.  **初始化 Memory Bank**:
    *   从 Cline 官网复制初始化 Memory Bank 的指令。
    
    (Link: https://docs.cline.bot/prompting/cline-memory-bank)
    *   将这些指令添加为项目的工作区规则（workspace rule）。
    *   在聊天框中运行 `/initialize memory bank` 命令来激活。
2.  **日常使用**: 初始化后，Memory Bank 会在后台自动工作。您在项目中进行的每个任务都会被记录和学习，为后续任务提供上下文。

---

## 3. /smol 命令
相关Youtube视频介绍： [Slash Commands Explained](https://www.youtube.com/watch?v=MxS5Jerpf-o)

**`/smol` 命令** 用于在保持关键信息的同时，压缩和精简当前的聊天上下文。这在处理长对话或探索性任务时尤其有用。

### 功能介绍
- **上下文压缩**: 将冗长的对话历史浓缩成一个简洁的摘要，保留核心的互动和决策。
- **节省 Token**: 在 LLM 上下文窗口有限的情况下，可以有效避免超出限制。
- **重新聚焦**: 当对话变得发散或重复时，使用 `/smol` 可以帮助您和 Cline 重新聚焦于核心任务，而无需从头开始。

### 使用方法
- **直接调用**: 在聊天框中输入 `/smol` 并执行。
- **多次使用**: 对于复杂的、探索性的任务，您可以多次使用 `/smol` 来不断精炼上下文，保持对话的高效性。

## 4. 快捷键
| Action                  | Windows/Linux | macOS   | Condition                    | Description                               |
| ----------------------- | ------------- | ------- | ---------------------------- | ----------------------------------------- |
| Add to Cline            | `Ctrl+'`      | `Cmd+'` | When text is selected        | Adds selected code to Cline chat          |
| Focus Chat Input        | `Ctrl+'`      | `Cmd+'` | When no text is selected     | Focuses the Cline chat input field        |
