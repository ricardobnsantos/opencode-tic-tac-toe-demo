# AGENTS.md

## Project Goal
Build a simple Tic-Tac-Toe project to demonstrate how to use OpenCode effectively.

This repository is for teaching.
The goal is not to build the most advanced version of the game.
The goal is to show a clean OpenCode workflow:
- start with a small request
- implement in small steps
- use planning before refactoring
- keep changes focused
- add tests when the logic becomes important

## Tech Constraints
- Use plain HTML, CSS, and JavaScript only
- Do not use frameworks
- Do not add unnecessary dependencies
- Keep the project runnable locally without a build step
- Keep the project small and easy to explain in a live demo

## Code Style
- Keep the code simple and beginner-friendly
- Use clear and descriptive names
- Prefer small, focused functions
- Avoid overengineering
- Avoid unnecessary abstraction
- Add comments only when they improve clarity

## Architecture Guidance
- Keep game logic separate from DOM updates when practical
- Preserve existing behavior unless a change is explicitly requested
- Prefer incremental changes over large rewrites
- Keep the number of files small

## UI Guidance
- Keep the UI clean and minimal
- Make the board easy to read and click
- Clearly show the current player
- Clearly show win and draw states

## Testing Guidance
- Add tests for core game logic when requested
- Focus tests on move validation, win detection, and draw detection
- Keep the test setup simple

## Behavior for Changes
- Make focused edits
- Avoid unrelated changes
- Briefly explain significant changes
- Do not introduce new tools or patterns unless explicitly asked