# babysitter

Orchestrate complex, multi-step workflows with event-sourced state management, hook-based extensibility, and human-in-the-loop approval

## Prerequisites

Install the Babysitter SDK CLI:

```bash
npm install -g @a5c-ai/babysitter-sdk
```

## Installation — Gemini CLI

```bash
npm install -g @a5c-ai/babysitter-gemini-cli
babysitter-gemini-cli install --global
```

Restart Gemini CLI to pick up the installed plugin.

## What's Included

- **Skills**: babysit
- **Hooks**: SessionStart, UserPromptSubmit, PreToolUse, PostToolUse, PreCompact, AfterAgent, SessionEnd, SessionIdle, ShellEnv
- **Commands**: (directory)

- **CLI**: Install/uninstall scripts for global and workspace setup



## Verification

```bash
babysitter harness:discover --json | grep gemini
```

## Integration Model

The plugin provides:

- Core orchestration skill for multi-step workflow management
- Lifecycle hooks for session state, orchestration loops, and token compression
- Command wrappers for plan, resume, doctor, and other operations

The process library is fetched and bound through the SDK CLI.
