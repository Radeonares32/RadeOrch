# RadeOrch

> Self-hosted, Rust-native AI agent orchestration and multi-project engineering management platform.

## Overview

RadeOrch is an engineering control plane designed to manage multiple software projects and orchestrate autonomous AI coding agents (Claude Code, OpenAI Codex, and local LLMs) with durable task execution, isolated Git worktrees, automated code review gates, and a lightweight web interface.

## Core Architecture

- **Backend:** Rust, Tokio, Axum, SQLx
- **Database:** PostgreSQL with advisory locking and transactional outboxes
- **Frontend:** Server-rendered HTML (Askama) + HTMX + Server-Sent Events (SSE)
- **Agent Execution:** Isolated Git worktrees, tmux terminal multiplexing, and containerized/sandbox execution
- **Workflows:** Multi-project kanban, local-first merge integration (`git merge-tree`), human-in-the-loop approval gates
