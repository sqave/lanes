<p align="center">
  <h1 align="center">Lanes</h1>
  <p align="center"><strong>Mission control for AI coding agents.</strong></p>
  <p align="center">Track, orchestrate, and ship across multiple AI CLI sessions from one place.</p>
</p>

<br>

## The Problem

You're running 3–5 AI agents in parallel across different features. You have 8 terminal tabs, no idea which one is doing what, and the only workflow tracker is your short-term memory. The AI agents got powerful — the workflow around them didn't.

## What Lanes Does

Lanes is a desktop app that gives you a kanban board where every card can have a live AI agent terminal attached. Drag work through stages. See what's running, what's blocked, and what shipped — all in one window.

- **Kanban workflow** — Issues move through Planning → Implementation → Review → Done. Drag to reorder, multi-select to bulk-manage.
- **Live terminals** — Each issue can have a running AI session with a real PTY. Click to expand, type to interact, drag files in.
- **Multi-agent orchestration** — Run multiple sessions concurrently with queue management. Lanes detects when one finishes and starts the next.
- **Auto-transitions** — Pattern matching on terminal output, CLI hooks, and file watchers detect when work moves to the next stage.
- **Dependencies** — Link issues that block each other. Cycle detection built in.
- **CLI-agnostic** — Works with Claude Code, Codex CLI, Gemini CLI, or any AI tool that runs in a terminal.
- **Metrics** — Token usage, cost tracking, and runtime duration per session.

## Install

```bash
brew install --no-quarantine sqave/lanes/lanes
```

Requires macOS Ventura or later. Runs natively on both Apple Silicon and Intel.

> The `--no-quarantine` flag is needed because Lanes is not notarized with Apple. It's safe — the app is open-source, ad-hoc signed, and runs entirely on your machine.

## Updates

Lanes checks for updates automatically on launch. You can also check manually in **Settings → About → Check Now**. No need to run `brew upgrade` — the app updates itself.

## Who It's For

- **Solo developers** running multiple AI agents in parallel across worktrees
- **Small teams** that need visibility into what's running and at what stage
- **Power users** who want a mission control layer without leaving the terminal

## How It Works

1. Create an issue describing what you want to build
2. Start a session — Lanes spawns your AI CLI in an isolated terminal
3. Work moves through your workflow as the agent progresses
4. See everything at a glance on the board. Click any card to jump into its terminal.

## Built With

Tauri 2, React 19, SQLite. Local-first, fast, private. Your code and data never leave your machine.

## License

Proprietary. All rights reserved.
