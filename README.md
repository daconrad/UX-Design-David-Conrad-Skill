# UX-Design-David-Conrad-Skill

---

# 🎨 UX Designer Skill (`SKILL.md`)

Transform AI coding agents and LLM workspaces into strategic UX design partners. This skill equips agents with senior interaction design heuristics, user journey mapping frameworks, wireframing scaffolds, and design system governance.

---

## 📌 Overview & Architecture

The `ux-designer` skill structures an agent's reasoning around user-centric design methodologies, ensuring generated UI recommendations, copy, and interaction patterns match enterprise-grade UX standards.

### Repository Layout

| Path | Purpose | Primary Artifacts |
|---|---|---|
| `SKILL.md` | Core instructions & prompt directives | System prompts, step workflows, evaluation rubrics |
| `references/` | Grounding knowledge & design standards | Heuristic checklists, accessibility (WCAG 2.2), token specs |
| `assets/` | Reusable output templates | ASCII wireframe grids, journey maps, user story schemas |
| `scripts/` | Tooling & verification hooks | Design token validation, accessibility contrast checkers |

---

## ⚡ Core Capabilities

| Capability | What It Does | Primary Output |
|---|---|---|
| **Heuristic Audit** | Evaluates workflows against Nielsen Norman & WCAG standards | Severity-ranked findings table with remediation steps |
| **Interaction Flow** | Maps user intent, system state, error states, and edge cases | State transition tables and step-by-step user journeys |
| **ASCII / Markdown Wireframing** | Scaffolds responsive layout wireframes in plain text | Structural UI blueprints with component hierarchy |
| **Design System Alignment** | Applies design tokens, component anatomy, and naming conventions | Token-mapped component specifications |
| **UX Copy & Microcopy** | Crafts contextual empty states, error strings, and button labels | Action-oriented copy alternatives with rationale |

---

## 🚀 Installation & Setup

Add this skill to your preferred agent runtime or IDE extension:

| Platform | Setup Instructions | Supported Features |
|---|---|---|
| **Cursor / Windsurf** | Copy `SKILL.md` into `.cursor/rules/` or workspace rules as `ux-designer.mdc`. | Context injection, active editing |
| **Claude Code / CLI** | Place in `.claude/skills/ux-designer/SKILL.md` or invoke via custom slash commands. | Autonomous tool execution, file reading |
| **Custom Agent / MCP** | Add directory path to your Agent configuration under skill manifests. | Full script execution, asset retrieval |

---

## 💡 How to Use the Skill

Trigger the skill using explicit role keywords or specific UX task queries.

| Intent | Example Prompt | Expected Deliverable |
|---|---|---|
| **Feature Conception** | *"Run a UX discovery session for an AI-assisted cloud capacity dashboard."* | Target personas, primary task flows, key telemetry requirements |
| **Wireframe Scaffolding** | *"Generate a high-density table wireframe for managing Kubernetes clusters."* | ASCII layout, column sorting hierarchy, bulk action bar |
| **Design Review** | *"Audit our checkout form modal for mobile accessibility and cognitive friction."* | Heuristic violation breakdown, contrast notes, tab order |
| **Error Handling** | *"Write microcopy and error resolution states for an API timeout scenario."* | Inline notification variants (retry, fallback, escalated support) |

---

## ⚙️ Customization & Parameters

Customize `SKILL.md` metadata frontmatter to align with your organization's design guidelines:

| Configuration Key | Allowed Values | Default | Purpose |
|---|---|---|---|
| `design_system` | `Material 3`, `Carbon`, `Polaris`, `Custom` | `Material 3` | Bases component anatomy and naming on target system |
| `fidelity` | `Low (Flows)`, `Medium (Wireframes)`, `High (Spec)` | `Medium` | Controls visual detail in ASCII/Markdown outputs |
| `target_user` | `Enterprise / Technical`, `Consumer`, `Developer` | `Enterprise / Technical` | Modulates cognitive density and interaction depth |
| `wcag_level` | `A`, `AA`, `AAA` | `AA` | Sets mandatory accessibility compliance threshold |

---

## 🤝 Contributing

We welcome additions to heuristic guides, new layout templates, and token mappings:

1. Fork the repository and create a feature branch (`feature/new-journey-template`).
2. Update `SKILL.md` or add corresponding references in `references/`.
3. Verify formatting and validate any python scripts via `scripts/run_checks.sh`.
4. Open a Pull Request detailing changes and sample agent conversation outputs.
