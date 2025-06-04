# Cursor User Rules — Vibecoding Best Practices

## 🧠 Thinking & Reasoning Rules
- After any context change (e.g., opening new files, running commands, or receiving outputs), pause and apply sequential thinking before responding.
- Use the think tool or structured reasoning in these cases:
  - After exploring files or project structure
  - After running commands or reviewing outputs
  - After receiving API/search results
  - When switching task parts
  - Before code suggestions or complex explanations
  - When reading PRD.md, UI.md, or todolist.md
- Always:
  - List relevant constraints and rules for the task
  - Gather all necessary information
  - Break down complex problems into clear steps
  - Analyze outputs thoroughly
  - Validate your plan before executing
  - Plan multi-step approaches in advance
  - Prompt the user if any part of the task is unclear

## 🗂 Project Kickoff Rules
- Before starting on a programming assignment:
  - Check for the presence of `PRD.md`, `UI.md`, and `todolist.md`
  - Use the think tool to thoroughly read and understand these documents
  - Prompt the user for clarification if anything is unclear
  - Always use **context7** MCP to align with best practices in:
    - Programming
    - API management
    - File/folder structure

## 💻 Coding Standards
- Always prefer simple, clean solutions
- Avoid code duplication by checking for existing similar functionality
- Write code considering dev, test, and prod environments
- Only make changes that are explicitly requested or clearly related
- When fixing bugs or issues:
  - Don’t introduce new patterns or tech without exhausting existing options
  - If new patterns are introduced, remove old implementations to avoid duplicates
- Keep the codebase clean and well-organized
- Avoid saving one-off scripts as permanent files
- Refactor files over **200–300 lines of code**
- Mock data only in tests; never in dev or prod
- Never add stubbing or fake data to dev or prod code
- Never overwrite `.env` without confirmation
- Focus only on code relevant to the task
- Don’t modify unrelated code
- Write thorough tests for all major features
- Avoid major pattern or architecture changes once a feature works well, unless explicitly instructed
- Always consider how your changes may affect other methods or code areas

## ⚙️ Implementation & Workflow Guidelines
- Always implement the most efficient and minimal code changes
- Comment each code section clearly to explain its purpose
- Code only within the **Docker** environment
- Never create new files; modify existing ones only
- After making changes, **always restart with a fresh server** to enable testing
- Before starting a new server, **kill all related existing servers** from previous tests
- Always try to **iterate on existing code or patterns** rather than create new ones or drastically change them
- **Rate-limit all APIs** appropriately
- Always create a `.gitignore` file and **ensure `.env` is included**

## 🎨 Frontend Development Guidelines
- When developing frontend components:
  - Use [shadcn UI](https://ui.shadcn.com/) and [HeroUI](https://www.heroui.com/) as references for components and UX inspiration
