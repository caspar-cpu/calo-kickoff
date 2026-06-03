# Calo Kickoff

A Claude Code plugin that everyone at Calo uses to **start a build**. It runs a rigorous
brainstorm (idea → design → spec → plan) and, on top of that:

- **Recommends Calo's approved tools** for your specific task, from a maintained register.
- **Flags anything off-list** — if your build (or an AI agent helping you) wants a tool
  that isn't approved, the plan tells you to speak to **Bohdan or Caspar** to get an
  admin-managed company account. Don't sign up for tools yourself.
- **Applies Calo's GitHub rules** so your resulting code ships into a company-connected,
  compliant repo: `master` branch, branch + PR with 2 approvals, no direct pushes, signed
  commits, files under 10MB, Internal-by-default visibility.

The brainstorming flow is adapted from [superpowers](https://github.com/obra/superpowers)
(MIT) — see [ATTRIBUTION.md](ATTRIBUTION.md).

## Install (company-wide)

In Claude Code:

```
/plugin marketplace add caspar-cpu/calo-kickoff
/plugin install calo-kickoff@calo
```

Then start any build by invoking the skill — it also triggers automatically when you
begin creating something:

```
/calo-kickoff:brainstorming
```

## What's inside

```
skills/brainstorming/
├── SKILL.md                      the brainstorming flow + the "Apply Calo standards" step
├── references/
│   ├── approved-tools.md         the approved-tools register
│   └── github-rules.md           Calo's GitHub Operational Guide & Rules
├── scripts/                      optional browser-based visual companion
├── spec-document-reviewer-prompt.md
└── visual-companion.md
```

## Maintaining the registers

The two files in `skills/brainstorming/references/` are the source of truth:

- **`approved-tools.md`** — to add, remove, or change an approved tool.
- **`github-rules.md`** — to update the GitHub rules.

Edit the file and open a PR (2 approvals, signed commits, into `master`). Changes reach
everyone when they next update the plugin.

## License

MIT — see [LICENSE](LICENSE). Brainstorming base © Jesse Vincent (Superpowers), MIT.
