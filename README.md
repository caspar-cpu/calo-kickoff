# Calo Kickoff

A Claude Code plugin that everyone at Calo uses to **start a build**. It has two parts:

1. **`kickoff`** — the [Superpowers](https://github.com/obra/superpowers) `brainstorming` skill, used **verbatim** (idea → clarifying questions → approaches → design → spec → plan). The proven methodology, untouched.
2. **`approved-tools`** — a background standards layer that runs *after* the build is scoped, at planning time. It recommends the Calo-**approved tools** for your build, names who to contact for access, and **writes the tools + Calo's GitHub rules into the implementation plan** — so the plan you approve *before coding* already specifies the signed-off stack and a compliant repo.

Off-list needs (including any tool an AI agent proposes mid-build) are flagged: don't sign up yourself — **speak to Bohdan or Caspar** for an admin-managed company account.

## Install (company-wide)

In Claude Code:

```
/plugin marketplace add caspar-cpu/calo-kickoff
/plugin install calo-kickoff@calo
```

(`/plugin` runs in **terminal Claude Code** or the Claude app's *Settings → Plugins* — not the in-app chat box.)

## How it flows

```
You: "I want to build X"
  → kickoff (verbatim Superpowers brainstorm): scopes the design + spec
  → approved-tools (at plan time): recommends the approved stack, writes it + the
    GitHub rules into the plan you review before coding
  → you build, on signed-off tools, in a Calo-connected repo
```

`kickoff` triggers automatically when you start creating something; `approved-tools` triggers once you're scoped and a plan is being written. Both can also be invoked explicitly (`/calo-kickoff:kickoff`, `/calo-kickoff:approved-tools`).

## What's inside

```
skills/
├── kickoff/                       Superpowers brainstorming, verbatim
│   ├── SKILL.md                   (only the frontmatter `name` + its own companion path differ)
│   ├── scripts/                   optional browser-based visual companion
│   ├── spec-document-reviewer-prompt.md
│   └── visual-companion.md
└── approved-tools/                Calo standards layer
    ├── SKILL.md
    └── references/
        ├── approved-tools.md      the approved-tools register
        └── github-rules.md        Calo's GitHub Operational Guide & Rules
```

## Maintaining the registers

The two files in `skills/approved-tools/references/` are the source of truth:

- **`approved-tools.md`** — to add, remove, or change an approved tool.
- **`github-rules.md`** — to update the GitHub rules.

Edit the file and open a PR (into `master`, 2 approvals, signed commits). Bump the version in `.claude-plugin/plugin.json` and `marketplace.json`, and people pick up the change by running `/plugin marketplace update calo`.

## License

MIT — see [LICENSE](LICENSE). The `kickoff` brainstorming skill is © Jesse Vincent (Superpowers), MIT — see [ATTRIBUTION.md](ATTRIBUTION.md).
