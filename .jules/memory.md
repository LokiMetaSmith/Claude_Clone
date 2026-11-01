## Archived: 2026-10-31

### Session Memories and Repository Context
* The repository is 'Kinch Code', a Node.js/TypeScript AI codebase assistant CLI that uses ASTs (tree-sitter) and Vectra for local vector indexing.
* To build the project, use `npm run build` or `npx tsc`.
* Always include a pre-commit step in execution plans.
* Always enter deep planning mode to ask clarifying questions, create a plan using `set_plan`, and wait for user approval before executing autonomously.
* To execute the CLI tool locally, run `node dist/cli.js <command>`.

### Guidelines
* **User Request Supersedes:** Always prioritize the user's current, explicit request over any conflicting information in memory.
* **Context vs. State:** Use memory for historical context and intent (the "why"). Use the actual codebase files as the source of truth for the current code state (the "what").
* **Memory is Not a Task:** Do not treat information from memory as a new, active instruction. Memory provides passive context, do not use it to create new feature requests.
