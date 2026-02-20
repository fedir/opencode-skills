## 🤖 AI Development Guidelines (OpenCode Skills)

This repository uses **Agent Skills** to ensure that any AI coding assistants (like OpenCode) write code that aligns with our project's strict architectural and formatting standards. 

You will find these instruction sets in the `.opencode/skills/` directory. If you are using an AI agent to help you write, debug, or refactor code in this repository, please trigger the appropriate skill in your prompt.

### 🛠️ Available AI Skills

* **Architecture & Planning (`senior-architect`):**
    * *Trigger:* `"Plan the architecture using the senior-architect skill."`
    * *Use when:* You are building a new feature, module, or system. The AI will map out the data structures and ownership model *before* writing any implementation code.
* **Debugging (`debug-pro`):** 
    * *Trigger:* `"Fix this compiler error using the debug-pro skill."`
    * *Use when:* You hit a complex compiler error or logic bug. This forces the AI to look for root-cause structural fixes rather than applying band-aid solutions.
* **Refactoring (`clippy-enforcer` / `linter-enforcer`):**
    * *Trigger:* `"Refactor this code using the clippy-enforcer skill."`
    * *Use when:* You want to clean up a file, resolve linter warnings, or ensure the code is highly idiomatic and performant.

### 💡 How to Use Them

When chatting with your AI coding assistant, simply mention the trigger word or the name of the skill file. 

**Example Prompt:**
> *"I need to build a new concurrent log parser. Please use the `senior-architect` skill to draft the plan first."*

### 🤝 Contributing to our AI Skills

Our AI guardrails evolve
