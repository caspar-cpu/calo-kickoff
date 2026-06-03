# Calo GitHub Operational Guide & Rules

The repository rules, visibility standards, and internal tools for the Calo GitHub organization. Any code you build at Calo follows these.

> 💡 **Flexibility note:** These are the org standard, but we are flexible. If a rule restricts your department's specific workflow, reach out to the admin team (Bohdan) to request a tailored setup for your repository.

## 🛑 The Golden Rule: connect your account first

**If you want to write, clone, or commit any code, it must live in a GitHub repository connected to the Calo corporate GitHub organization.** Bohdan organises this. Before you write or commit anything, your account and repositories must be connected to the Calo org via Bohdan.

This is mandatory. It is how we observe what is being written and built — for support, security, IP ownership, and consistency. No code should be built outside the company GitHub.

## 🔒 The 5 core GitHub rules

1. **File size limit (<10MB).** Do not push files larger than 10 MB to Git. Keep datasets and heavy media assets outside the repository.
2. **Primary branch is `master`.** We use traditional naming. The default production branch is `master`, not `main`.
3. **2-approval PR requirement.** You cannot merge alone. Every pull request requires two (2) approved reviews from team members before it can be merged into the default branch.
4. **No direct pushes to `master`.** Direct pushes to `master` are blocked across all repositories. All updates go through a separate branch and a PR.
5. **Signed commits only.** Every commit must be cryptographically signed using a key generated and linked to your GitHub profile. Unsigned commits are automatically rejected.

🔑 Organization admins retain overarching access to all repositories (Public, Private, and Internal) for compliance and management purposes.

## 👁️ Repository visibility standards

- **Internal (default).** Visible and searchable to everyone in the Calo GitHub organization. Use for general company projects and collaboration.
- **Private.** Restricted to specific individuals or a single department. Use for sensitive data or restricted projects.
- **Public.** Open to the entire internet. Strictly reserved for open-source initiatives or public-facing code.

## 🛠️ Key internal repositories & tools

- **`install`** — Start here. A single script that automatically configures your entire local machine environment, including local Git settings. Removes the need for manual setup.
- **`copilot`** — Our internal, custom LLM plugin used to assist with AI generation and developer workflows.
- **`goui`** — Our central internal design system repository. Standard company UI elements and design components live here.
- **`actions`** — A library of reusable GitHub Actions, primarily used by core engineering for CI/CD automation workflows.

## How this applies to anything you build

When you plan and build with an AI agent, the resulting code must:

- live in a repository **connected to the Calo org** (contact **Bohdan** to connect your account/repo first if it isn't already), and
- follow the 5 core rules above — `master` branch, branch + PR with 2 approvals, no direct pushes, signed commits, files under 10MB — at the **Internal** default visibility unless it is genuinely open-source.
