# PiCoder Monorepo - AGENTS.md

> Map, not encyclopedia. This file points to deeper sources.

## Essential Rules

### Code Quality
- No `any` types unless absolutely necessary
- NEVER remove or downgrade code to fix type errors; upgrade the dependency instead

### Commands
- After code changes: `npm run check` (get full output, no tail)
- **NEVER run**: `npm run dev`, `npm run build`, `npm test`
- **NEVER commit unless user explicitly asks**

### Style
- Keep answers short and concise, no emojis
- Technical prose only, be kind but direct

## Repository Structure

```
picoder/
├── packages/
│   ├── ai/              # Multi-provider LLM API
│   ├── agent/           # Core agent runtime
│   ├── coding-agent/    # Interactive coding CLI (pi)
│   ├── mom/             # Slack bot
│   ├── pods/            # vLLM deployments CLI
│   ├── tui/             # Terminal UI library
│   └── web-ui/          # Web components
└── docs/
    ├── design-docs/     # Architecture decisions
    ├── exec-plans/      # Active & completed plans
    ├── references/      # Operational knowledge
    └── product-specs/   # Requirements
```

## Where to Find Things

| Topic | Location |
|-------|----------|
| Contribution & git workflow | `docs/references/contribution.md` |
| Coding rules | `docs/references/coding-rules.md` |
| Commands reference | `docs/references/commands.md` |
| Testing guidelines | `docs/references/testing.md` |
| Release process | `docs/exec-plans/releasing.md` |
| Adding LLM providers | `docs/design-docs/new-llm-provider.md` |

## Design Principles

- Design docs define architecture decisions
- Exec plans track implementation progress
- References contain operational knowledge (never in your head)
