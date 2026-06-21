# Cursor Project Guide

Instructions for AI agents working in this repository.

## Project Overview

- **Name:** ai-file
- **Stack:** Node.js (CommonJS), HTML
- **Dependencies:** `dotenv` for environment variables

This is a small workspace for experiments, HTML pages, and lightweight Node scripts.

## Structure

```
.
├── cursor.md          # This file — agent instructions
├── README.md          # Project overview
├── package.json       # Node.js config
├── hell nah.html      # Sample HTML page
└── node_modules/      # Dependencies (do not edit)
```

## Coding Conventions

- Use **CommonJS** (`require` / `module.exports`) for Node.js code unless the project is migrated to ESM.
- Keep HTML files self-contained (inline CSS/JS is fine for small pages).
- Load secrets via `dotenv`; never commit `.env` files or hardcode API keys.
- Prefer minimal, focused changes. Match the style of existing files.

## Environment Variables

- Store secrets in a `.env` file at the project root.
- Access them with `require('dotenv').config()` at the top of entry scripts.
- Document required variables in comments or README when adding new ones.

## What to Avoid

- Do not modify `node_modules/`.
- Do not add heavy frameworks unless explicitly requested.
- Do not create commits unless the user asks.

## Common Tasks

| Task | Approach |
|------|----------|
| New HTML page | Add a `.html` file in the project root or a dedicated folder |
| Node script | Add a `.js` file and wire it in `package.json` scripts if needed |
| Env config | Use `dotenv`; add a `.env.example` with placeholder values |
