# Cline Usage Tips
This document introduces some common and practical small features that I find useful in my short-term use.
---

## 1. Plan and Act Mode
Related official YouTube video: [How to Use Plan & Act Modes in Cline](https://www.youtube.com/watch?v=b7o6URFPp64)

**Plan and Act Mode** divides the development process into two stages, aiming to reduce subsequent modifications through thorough upfront planning, thereby saving time and tokens.

### Feature Introduction
- **Plan Mode**: In this mode, you can communicate deeply with Cline to clarify task requirements, explore different solutions, and formulate detailed execution strategies. In this stage, Cline acts like a project manager, using its search, file reading, and analysis capabilities to plan the best path for you. This stage usually involves using models with strong reasoning abilities and large context windows, as the cost of the planning phase is relatively low.
- **Act Mode**: Once you are satisfied with the plan, you can switch to Act Mode. Cline will strictly execute the strategies and context established in Plan Mode. In this stage, you can switch to a model that is better at coding, thus combining the advantages of both models: one for strategic planning and one for code implementation.

### How to Use
1.  **Enter Plan Mode**: When starting a new task, actively switch to Plan Mode.
2.  **Detailed Communication**: Communicate your requirements fully with Cline, letting it read relevant files, search documents, and propose an implementation plan.
3.  **Confirm the Plan**: After you confirm that Cline fully understands the task and has formulated a reliable plan.
4.  **Switch to Act Mode**: Switch to Act Mode, and you can choose a model more suitable for coding to execute the plan.

---

## 2. Memory Bank
Related official YouTube video: [Ideal Setup for Cline](https://www.youtube.com/watch?v=UBqh6ud5LqY)

**Memory Bank** is a technique that allows Cline to share and remember context across different tasks within the same project. It ensures that when handling new tasks, Cline can "remember" the project's history, technological choices, and overall direction.

### Feature Introduction
- **Cross-Task Memory**: Solves the problem of repeatedly providing project background information when starting a new task.
- **Maintain Consistency**: Ensures that Cline's output is consistent with the project's existing standards and architecture.
- **Project Evolution**: Helps Cline understand the project's evolution process, thereby providing more relevant suggestions and code.

### How to Use
1.  **Initialize Memory Bank**:
    *   Copy the Memory Bank initialization instructions from the Cline official website.
    (Link: https://docs.cline.bot/prompting/cline-memory-bank)
    *   Add these instructions as a project workspace rule.
    *   Run the `/initialize memory bank` command in the chatbox to activate it.
2.  **Daily Use**: Once initialized, the Memory Bank will work automatically in the background. Every task you perform in the project will be recorded and learned, providing context for subsequent tasks.

---

## 3. /smol Command
Related YouTube video introduction: [Slash Commands Explained](https://www.youtube.com/watch?v=MxS5Jerpf-o)

The **`/smol` command** is used to compress and streamline the current chat context while retaining key information. This is particularly useful when dealing with long conversations or exploratory tasks.

### Feature Introduction
- **Context Compression**: Condenses a lengthy chat history into a concise summary, preserving core interactions and decisions.
- **Save Tokens**: Effectively avoids exceeding limits when the LLM's context window is limited.
- **Refocus**: When a conversation becomes divergent or repetitive, using `/smol` can help you and Cline refocus on the core task without starting over.

### How to Use
- **Direct Call**: Type `/smol` in the chatbox and execute it.
- **Multiple Uses**: For complex, exploratory tasks, you can use `/smol` multiple times to continuously refine the context and maintain conversation efficiency.

## 4. Shortcuts
| Action                  | Windows/Linux | macOS   | Condition                    | Description                               |
| ----------------------- | ------------- | ------- | ---------------------------- | ----------------------------------------- |
| Add to Cline            | `Ctrl+'`      | `Cmd+'` | When text is selected        | Adds selected code to Cline chat          |
| Focus Chat Input        | `Ctrl+'`      | `Cmd+'` | When no text is selected     | Focuses the Cline chat input field        |
