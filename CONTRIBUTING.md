# Contributing to the NovaHub Network

Thank you for helping build NovaHub. This document explains our contribution process, issue and label conventions, project board workflow, and the custom fields used on the NovaHub Development Roadmap.

Please read this file and any repository-specific CONTRIBUTING notes before opening issues or PRs. For general community behaviour, see [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md).

---

## Understanding the digital ecosystem

The NovaHub project is composed of several key public assets. Knowing where everything lives makes contributions effective.

| Asset | Primary audience | Core purpose | Key content | Primary CTA(s) |
|---|---|---|---|---|
| [circular.engineering/novahub](https://circular.engineering/novahub) | Business stakeholders, potential customers, investors | Announce the project from a corporate perspective and explain the business case and how it relates to company vision. | High-level overview, business benefits, link to project site, enterprise support info (future). | Explore the Project / Visit novahub.network |
| [novahub.network](https://novahub.network) | Potential contributors, users, evaluators | Main public portal and gateway to collaboration; attracts and engages the open-source community. | Project mission, features, demos/screenshots, contributor info, links to GitHub and Docs. | Contribute on GitHub / Read the Docs |
| [novahub.network/docs/](https://novahub.network/docs/) | Developers (contributors & users) | Comprehensive technical documentation for using and contributing to NovaHub. | Getting started, API reference, architecture diagrams, contribution process. | Navigate and search |
| [app.novahub.network](https://app.novahub.network) | Active users | The interactive NovaHub product. | Product dashboards, creation tools, user interfaces. | Create Project / Login |
| [GitHub Organization](https://github.com/novahub-network) | Active contributors, maintainers | Host source code, manage issues, and review contributions via Pull Requests. | Source code, Issues (including Good First Issues 🌱), Pull Requests, CONTRIBUTING.md. | Fork repository / Submit an issue |
| [Product Development Roadmap](https://github.com/orgs/novahub-network/projects/1) | Active & potential contributors | Visualize the development roadmap, track high-level features, and manage non-code tasks. | Task cards, progress columns (Triage, Ready, In Progress, In Review, Done), contribution guidance. | Claim a task / View the roadmap |
| [Product Discussions](https://github.com/orgs/novahub-network/discussions/) | Community members (users & contributors) | Host brainstorming, Q&A, and early-stage idea refinement before work is scoped into issues. | Feature ideas, questions, announcements, polls, community conversation. | Start a discussion / Answer a question |

Use this section to orient yourself: pick the asset that matches your goal (documentation, contribution, or product use), then follow the links and conventions described below.

---

## Issue Types (GitHub standard)

Across NovaHub we use the standard GitHub Issue Type values (selected when creating an issue or PR):

- Task  
- Bug  
- Feature

Set the correct Type when creating an issue so items can be filtered and mapped to Projects automatically.

---

## Official label set

We maintain a small, consistent set of organization-wide labels. Exact spelling and emoji are part of the canonical names; these labels are enforced via our label sync.

| Label | Purpose |
|---|---|
| **good first issue 🌱** | Simple, well‑scoped tasks ideal for newcomers. |
| **help wanted 🤝** | Open for contribution: maintainers welcome external help. |
| **blocked ⛔** | Work cannot proceed due to external dependency. |
| **hotfix 🔥** | Urgent fix required for production stability. |
| **needs design 🖌️** | Requires UX/UI design input. |
| **needs dev 💻** | Requires coding or engineering expertise. |
| **needs docs 📝** | Requires technical writing or documentation updates. |
| **needs expert-input 🎯** | Needs input from a subject matter expert. |
| **needs legal 📜** | Requires legal or compliance review. |
| **needs pm 📊** | Requires product management input for scope/clarity. |

Do not create organization-wide labels outside this set without discussing with maintainers. Repository-local labels may exist for local workflows but keep them minimal to provide a consistent contributor experience.

---

## Filter by your skills using labels

Filter issues and the roadmap by the labels that describe the skills or input required. This helps you quickly find work that matches your strengths.

- **needs docs 📝** — Requires technical writing or documentation updates.  
- **needs design 🖌️** — Needs UX/UI or visual design input.  
- **needs dev 💻** — Requires coding or engineering expertise.  
- **needs expert-input 🎯** — Needs subject-matter expertise or technical review.  
- **needs legal 📜** — Requires legal or compliance review.  
- **needs pm 📊** — Requires product management input for scope, acceptance criteria, or prioritization.

Tip: Combine a `needs` label with a `Type` and `Status` to narrow results (for example, filter for `needs docs 📝` + `Ready` to find documentation tasks that are ready to pick up).

---

## NovaHub Development Roadmap: project fields and Status

The public roadmap is the canonical planning view for NovaHub:  
https://github.com/orgs/novahub-network/projects/1/

The roadmap uses a Kanban board and specific project custom fields. These fields are authoritative for planning and filtering on the roadmap.

Project custom field — Status (maps to columns)
- **Triage** — The inbox for new issues. Maintainers review, label, and prioritize items here. This is not for contributors to pick work from.
- **Ready** — Fully scoped and prioritized issues ready for contributors to pick up.
- **In Progress** — Issues that have been assigned and are actively being worked on.
- **In Review** — Issues with an open Pull Request awaiting review. This will be automated where possible.
- **Done** — Pull Requests have been merged and the work is complete.

Other project custom fields
- **Priority** — {Critical 🚨, High 🔥, Medium ⚖️, Low 💤}  
- **Difficulty** — {Hard 🔴, Medium 🟡, Easy 🟢}  
- Additional fields in use: **Team**, **Iteration**, **Quarter**

When creating or updating issues, maintainers will set Type, Status, Priority, and Difficulty. Contributors should respect those settings when claiming work.

---

## How triage works

- New issues land in **Triage**. Maintainers review, add labels from the official set, set Type, Priority and Difficulty, and move the item to the appropriate Status.
- Only issues in **Ready** should be taken by unassigned community contributors.
- To claim an issue: comment on it to say you want it; a maintainer will assign and move it to **In Progress**.
- When you open a PR for an assigned issue, project automation will move the project item to **In Review**; after merge it moves to **Done**.

---

## Mapping labels to Project fields

We keep labels as the canonical, org‑wide metadata and map them to Project fields where appropriate:

- The label family (e.g., `needs dev 💻`) describes required skills and is visible on issues.
- The Project field **Type** (Task/Bug/Feature) remains the project-level enum used in roadmap filters and is set on issue creation.
- Project custom fields (Status, Priority, Difficulty) are authoritative for the roadmap and are set by maintainers during triage.

We run automation to keep labels and project fields aligned. If you work on automations or need to change mappings, coordinate with maintainers.

---

## Finding something to work on

- Start in [Product Discussions](https://github.com/orgs/novahub-network/discussions/) for ideas and brainstorming.  
- Actionable tasks are tracked on the public [Product Development Roadmap](https://github.com/orgs/novahub-network/projects/1).  
- Good starting points:
  - [Good First Issues 🌱 view](https://github.com/orgs/novahub-network/projects/1/views/6) — beginner-friendly tasks.  
  - [Kanban Ready column](https://github.com/orgs/novahub-network/projects/1/views/4) — scoped and prioritized issues ready to pick up.  
- Filter by labels that match your skills (see Filter by your skills using labels above).

---

## Code contribution workflow

1. Fork the repository you want to contribute to.  
2. Clone your fork: `git clone <your-fork>`.  
3. Create a branch: `git checkout -b my-new-feature`.  
4. Make changes, run tests, and commit with clear messages.  
5. Push your branch to your fork.  
6. Open a Pull Request to the original repository and link the issue it resolves.

PR checklist
- Link to the issue (use closing keywords if appropriate).  
- Ensure Type, Status, Priority, and Difficulty are set or noted.  
- Follow repo-specific guidelines: CI, tests, linters, and code style.  
- Write a clear PR description and testing notes.

---

## Documentation and design contributions

- Use **needs docs 📝** for documentation tasks and **needs design 🖌️** for design work.  
- For large documentation proposals, open an issue so it can be triaged and scheduled.  
- Provide screenshots, examples, or sample copy where helpful.

---

## Legal, expert-input, and PM review

- If domain expertise is required, add **needs expert-input 🎯**.
- For compliance or legal review, add **needs legal 📜**.
- For scope or product-level decisions, add **needs pm 📊**.

---

## Label and project hygiene

- We run an org-wide label sync from `.github/labels.json`. Do not rename official labels locally; open an issue in this repo to discuss changes.  
- Migration/cleanup process: new canonical labels are added to `.github/labels.json`, aliases are renamed to canonical names by automation, and stray labels are removed after a grace period.  
- Avoid deleting labels that are referenced in automation or CI without coordination. If you believe a label should be removed, open an issue in `.github`.

---

## Questions, help, and escalation

- Unsure where to start? Open a discussion or comment on the issue and ping a maintainer.  
- For questions about process, labels, or project mappings, open an issue in this `.github` repository.

---

## Thank you

Your contributions move NovaHub forward. Thank you for your time, attention to detail, and collaboration.