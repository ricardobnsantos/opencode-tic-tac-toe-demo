# OpenCode Tic-Tac-Toe Demo

This repository is a small teaching project designed to demonstrate how to use OpenCode effectively on a simple codebase.

The goal is not to build the most advanced Tic-Tac-Toe game.  
The goal is to show a clean workflow for working with OpenCode:
- define repository instructions
- implement in small steps
- use planning before refactoring
- keep prompts short and focused
- add tests when the logic becomes important

## Prerequisites

Before using this repository, you should have:

- OpenCode installed
- access to OpenCode in your terminal or preferred environment
- a GitHub account if you want to clone, fork, or share the repository

This demo assumes you already know how to open a repository with OpenCode.

## What this demo shows

This demo is meant to teach:
- how to give OpenCode project context through `AGENTS.md`
- how to structure implementation with an `implementation-plan.md`
- how to use short prompts when the repository already contains instructions
- how to use planning before structural changes
- how to work incrementally instead of asking for everything at once

## Repository structure

```text
.
├── AGENTS.md
├── opencode.json
└── docs/
    └── implementation-plan.md
```

### `AGENTS.md`
Defines the main repository rules:
- project goal
- tech constraints
- coding style
- architecture guidance
- UI guidance
- testing guidance
- expectations for future changes

### `docs/implementation-plan.md`
Defines the implementation phases for the demo:
1. minimal playable version
2. core game rules
3. restart flow
4. refactor for clarity
5. tests
6. optional enhancement

### `opencode.json`
Loads `docs/implementation-plan.md` as an additional instruction file for OpenCode.

## How to use this demo

1. Clone this repository
2. Open it with OpenCode
3. Start with the planning step
4. Follow the prompts below in order
5. Review the results after each step instead of jumping ahead

## Step-by-step demo prompts

### Step 0 — Review repository context

Use `plan` first to show that OpenCode can read and understand the repository instructions before making changes.

```text
@plan Review the repository instructions and summarize:
- the project goal
- the technical constraints
- the implementation phases
- the coding expectations

Do not modify any code.
Keep the summary short and practical.
```

### Step 1 — Implement Phase 1

```text
Implement Phase 1 from docs/implementation-plan.md.
Follow the project instructions.
Keep the implementation simple and beginner-friendly.
```

### Step 2 — Implement Phase 2

```text
Implement Phase 2 from docs/implementation-plan.md.
Preserve the current structure unless changes are necessary.
```

### Step 3 — Implement Phase 3

```text
Implement Phase 3 from docs/implementation-plan.md.
Keep the UI simple and consistent with the current design.
```

### Step 4 — Plan the refactor

Use `plan` before making structural changes.

```text
@plan Review the current implementation and Phase 4 from docs/implementation-plan.md.

Suggest a small refactor plan to:
- separate game logic from DOM updates
- improve readability
- keep the code beginner-friendly
- preserve visible behavior

Do not modify the code.
```

### Step 5 — Apply the refactor

```text
Implement the refactor you proposed for Phase 4.
Preserve visible behavior and avoid overengineering.
Briefly explain the main structural changes.
```

### Step 6 — Add tests

```text
Implement Phase 5 from docs/implementation-plan.md.
Use a simple test setup and explain how to run the tests locally.
```

### Step 7 — Optional planning for one final enhancement

```text
@plan Review the current project and recommend the best next small enhancement for this demo.

Choose one option only:
- scoreboard
- random computer opponent
- small UI polish

Explain your recommendation briefly.
Do not modify the code.
```

### Step 8 — Implement the chosen enhancement

If the recommendation is a scoreboard:

```text
Implement a simple scoreboard.
Keep the UI simple and preserve the current structure unless changes are necessary.
```

If the recommendation is a computer opponent:

```text
Implement a very simple optional computer opponent.
Keep the code easy to understand and avoid unnecessary complexity.
```

### Step 9 — Final cleanup

```text
Review the current project and make a final cleanup pass.

Focus on:
- readability
- small naming improvements
- minor duplication removal
- preserving behavior
- keeping the code beginner-friendly

Do not perform a large rewrite.
Summarize the final improvements briefly.
```

## Suggested teaching flow

A good live flow for this demo is:

1. explain the repository structure
2. explain why `AGENTS.md` exists
3. explain why `implementation-plan.md` exists
4. show `plan` reading the repository context
5. implement the project phase by phase
6. use `plan` again before refactoring
7. add tests
8. optionally add one small enhancement
9. close with the main lessons

## Key teaching points

The main ideas behind this demo are simple:

- repository context matters
- prompts should be short and specific
- implementation should happen in small steps
- `plan` should be used before structural changes
- the agent should not be asked to do everything at once

## Why Tic-Tac-Toe?

Tic-Tac-Toe is a good teaching project because it is:
- small
- visual
- easy to understand
- easy to validate
- simple enough for a short demo
- rich enough to demonstrate iteration, refactoring, and testing

## Why this repository is public

This repository exists so other people can:
- inspect the setup
- reuse the structure
- run the same demo
- adapt the workflow for their own OpenCode projects

## Note about larger workflows

For a small teaching demo, OpenCode on its own is the right starting point.

If the project were larger, or if a more spec-driven workflow with stronger context engineering were needed, a layered approach using something like Get Shit Done could make sense.  
But this repository intentionally focuses on teaching OpenCode itself first.

## License

Add the license you prefer for sharing and reuse.
