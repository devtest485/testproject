# AGENTS.md

## Project Type
Next.js / React - App Router

## AI Agent Policy

This repository follows the [Simple-AI-Workflow](https://github.com/FaziHamza/Simple-AI-Workflow) protocol for AI-assisted development.

## Session Protocol

1. **Before starting**: Read `ai/context.md` and `ai/next-steps.md`
2. **During work**: Make focused changes and keep the user informed
3. **Before committing**: Ask the user whether the changes should be committed
4. **If commit is approved**: Ask whether to commit on a new branch or on the current/default working branch
5. **After completing**: Update `ai/progress.md` and `ai/next-steps.md`
6. **End of session**: Create a checkpoint in `ai/daily-checkpoints/`

## Constraints

- Do not push directly to `main` without human review
- Do not create commits without explicit user approval
- After commit approval, confirm whether to use a new branch or the current/default working branch
- Prefer a feature branch for non-trivial changes unless the user chooses the current/default working branch
- Keep commits atomic and descriptive
- Do not modify files outside the scope of the current task
- Never expose secrets, tokens, or credentials in commits

## Stack-Specific Guidance

- Keep routes and server components in `app/`
- Keep reusable UI in `components/`
- Use Server Components by default; add `"use client"` only when interactivity requires it
- Use Tailwind CSS utility classes and existing design tokens before adding new styling patterns
- Keep TypeScript strict; avoid `any` unless there is a clear reason
- Keep API routes in `app/api/` with explicit validation and error handling
- Never expose secrets or tokens in client-side code

## Tracking Files

| File | Purpose |
|------|---------|
| `ai/context.md` | Repository purpose and key structure |
| `ai/progress.md` | Session progress log |
| `ai/next-steps.md` | Pending tasks and resume point |
| `ai/daily-checkpoints/` | Daily session summaries |

## Getting Started

Run **Bootstrap AI** from AgentBoard to create the `ai/` tracking folder structure.
