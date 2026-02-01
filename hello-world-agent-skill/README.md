# Hello World Agent Skill 🌍

Welcome to your first **Agent Skill**! This repository serves as a simple demonstration and a beginner-friendly tutorial on how to extend the capabilities of your AI agent.

## 🎯 What is this?
An **Agent Skill** is a package that teaches your AI assistant new tricks. It consists of:
1.  **`SKILL.md`**: The instruction manual for the AI.
2.  **Scripts**: The actual code (Bash, Python, etc.) that performs the task.

## 📦 Installation (Universal Method)

To make this skill work automatically with **both** Gemini Code Assist and Claude Code, follow this standard structure:

1.  Create a `.claude/skills` folder in your project root (if it doesn't exist).
2.  Clone this repository into that folder.

```bash
mkdir -p .claude/skills
cd .claude/skills
git clone https://github.com/sasha-0134/agent-utils.git
```

### Why this location?
*   **Claude Code CLI**: Strictly requires skills to be in `.claude/skills` to see them automatically.
*   **Gemini CLI**: Fully supports this standard and will also detect skills here.

By putting it here, you get a **Universal Skill** that works everywhere! 🌍

## 🚀 Usage
Once this folder is in your project workspace, you can simply ask your agent:

> "Run the hello world skill"
> "Test the hello tool"

The agent will read `SKILL.md`, find the instruction to run `scripts/hello.sh`, and execute it for you.

## 🛠️ How to Customize
You can use this skill as a template for your own ideas:

1.  **Edit the Logic**: Open `scripts/hello.sh` and change the code to do whatever you want (e.g., check system stats, fetch a joke, deployment scripts).
2.  **Update the Brain**: Edit `SKILL.md` to describe your new tool so the agent knows when to use it.

## 📂 Structure
- `SKILL.md`: Defines the tool `hello` and how to use it.
- `scripts/hello.sh`: A simple script that prints a cool ASCII art greeting.

---
> 💡 **Tip**: Try modifying the ASCII art in `scripts/hello.sh` to make it your own!
