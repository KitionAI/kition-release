# Kition

Kition is a local-first AI workspace for notes, structured data, and autonomous work.

It combines an Obsidian-style Markdown editor, Notion-style data tables, and an AI agent that can read files, edit documents, run commands, browse the web, and work with external tools. Your workspace stays on your own machine, in a vault directory you choose.

Website: https://kition.ai

## What Kition Is

Kition brings three primitives into one desktop workspace:

| Primitive | What it gives you |
| --- | --- |
| Markdown documents | Plain `.md` files on disk, edited with a CodeMirror 6 surface that supports live preview, wikilinks, callouts, math, diagrams, and a command palette. |
| Structured tables | Notion-style fields, views, and records that live next to your documents in the same vault. Use them for content calendars, CRMs, task boards, research indexes, and asset libraries. |
| AI agent | A tool-using agent that can read and write files, patch documents, run shell commands, browse the web with a real Chromium session, query MCP servers, and operate on data tables. |

Kition is designed for people who want local files, real structure, and an AI assistant that can do more than chat.

## Core Features

### Local-first vaults

Your data lives in a normal folder on your machine.

- Documents are plain Markdown files.
- Tables are portable Kition table files and can be imported or exported.
- Vaults can be backed up with Git, Time Machine, iCloud, OneDrive, or any file sync system you already trust.
- No cloud account is required for the base desktop flow.

### Markdown editor

Kition's editor is built for long-form work without locking your content into a proprietary block format.

- Live preview with an Obsidian-style writing experience.
- `[[wikilinks]]`, backlinks, embeds, callouts, math, Mermaid, and code blocks.
- Command palette for common actions.
- Markdown toolbar and keyboard shortcuts.
- The same vault can still be opened in Obsidian, VS Code, Vim, or any text editor.

### Structured data tables

Tables sit beside your prose instead of living in a separate SaaS product.

- Field types for text, rich text, number, date, select, multi-select, URL, attachment, formula, and AI fields.
- Grid, Kanban, Gallery, and Calendar views.
- CSV import and export.
- Inline document references and table embeds.
- Agent-readable and agent-writable records.

### AI agent

The Kition agent is built as a workspace operator, not a decorative chat panel.

- Reads, searches, and edits files across the vault.
- Applies document changes as patches so edits are reviewable.
- Runs shell commands when the task needs local execution.
- Uses a real Chromium browser for pages that require JavaScript, login sessions, or interactive workflows.
- Reads and writes structured tables through first-class tools.
- Supports plan and goal workflows for larger tasks.

### Extensible by design

Kition can connect to the rest of your stack.

- Bring your own model provider: OpenAI-compatible endpoints, OpenAI, Anthropic, or custom providers.
- Connect MCP servers for tools such as GitHub, Linear, Notion, Postgres, Slack, or internal APIs.
- Add Hooks around agent lifecycle events and tool calls.
- Use subagents for parallel research, review, or batch work.
- Add custom local tools for workflows that are specific to your team.

## Who It Is For

- Writers and creators who want drafts, research, outlines, calendars, and AI assistance in one vault.
- Researchers who need Markdown notes, structured reading lists, citations, and summarization workflows.
- Developers and tinkerers who want a local AI workbench that can use files, commands, browser sessions, MCP, and custom tools.
- Small teams and agencies that manage client docs, content calendars, asset libraries, and lightweight CRMs.
- Anyone who wants the power of an AI workspace without moving their source of truth into a cloud-only product.

## Getting Started

1. Download and open the Kition desktop app from https://kition.ai.
2. Choose or create a local folder as your vault. Existing Markdown folders work.
3. Open Settings and add an AI provider key if you want agent and AI-field features.
4. Start writing documents, creating tables, or asking the agent to work inside your vault.

Kition can be used without an account for local desktop workflows. AI calls use the provider you configure.

## Data And Privacy

Kition is built around local ownership.

- Your vault stays in the directory you selected.
- Markdown files remain plain `.md`.
- API keys are intended to be stored through the operating system credential store.
- The desktop app does not require cloud sync to operate.
- Features that call an AI provider or fetch web content may send the relevant prompt, context, or request to the provider you configured.

## Platform Support

Kition is a desktop app built with Electron and a Go sidecar service.

Current target platforms:

- macOS
- Windows
- Linux

## Open Source

This repository is the public home for Kition releases and open-source distribution work.

The product direction is simple: keep knowledge work local, make structured data first-class, and give the AI agent real tools so it can complete useful work inside the workspace.
