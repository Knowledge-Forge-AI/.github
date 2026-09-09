# Knowledge Forge AI

Knowledge Forge AI builds deterministic, inspectable tools for agent engineering and human-reviewable software and design workflows.

Our public work currently centers on two complementary areas:

- **Agent engineering** — bounded, provider-neutral tooling for skills, evidence, environment capture, repository analysis, and reproducible agent workflows.
- **Theme Forge** — deterministic tooling for vector assets, brand systems, documentation themes, and local visual-design workbenches.

> Project-specific READMEs, release notes, licenses, and contribution files are the source of truth for each repository's current maturity, compatibility, distribution, licensing, and contribution requirements.

## Table of contents

### Public projects and repositories

1. [Agentic Praxis Grimoire](#agentic-praxis-grimoire)
2. [Theme Forge Stellar Burst](#theme-forge-stellar-burst)
3. [Theme Forge Nebular Fusion](#theme-forge-nebular-fusion)
4. [Theme Forge Stellar Loom](#theme-forge-stellar-loom)
5. [Starlight Theme Terminal Nova](#starlight-theme-terminal-nova)
6. [Knowledge Forge AI Website](#knowledge-forge-ai-website)
7. [Organization Community Health](#organization-community-health)

### About Knowledge Forge AI

- [How the projects fit together](#how-the-projects-fit-together)
- [Project status](#project-status)
- [Licensing model](#licensing-model)
- [Contributing](#contributing)

## Public projects and repositories

### Agentic Praxis Grimoire

**Repository:** [Knowledge-Forge-AI/agentic-praxis-grimoire](https://github.com/Knowledge-Forge-AI/agentic-praxis-grimoire)

Agentic Praxis Grimoire (APGR) is a provider-neutral toolkit and skill corpus for bounded agent engineering. It supplies deterministic primitives for task-scoped skill selection, evidence capture, curated environment snapshots, repository analysis, and context-footprint accounting without imposing a particular orchestration system.

APGR is intended to be consumed by coding-agent platforms, LLM harnesses, agentic workflows, and orchestrators rather than acting as an autonomous agent itself.

### Theme Forge Stellar Burst

**Repository:** [Knowledge-Forge-AI/theme-forge-stellar-burst](https://github.com/Knowledge-Forge-AI/theme-forge-stellar-burst)

Theme Forge Stellar Burst (TFSB) is a deterministic declarative SVG compiler, transactional installer, and lifecycle drift checker. It turns a bounded SVG subset into human-editable TOML, compiles canonical SVG output, distributes assets to configured destinations, and helps reconcile upstream changes without silently overwriting human edits.

### Theme Forge Nebular Fusion

**Repository:** [Knowledge-Forge-AI/theme-forge-nebular-fusion](https://github.com/Knowledge-Forge-AI/theme-forge-nebular-fusion)

Theme Forge Nebular Fusion is a local desktop workbench for reviewing, inspecting, and managing Theme Forge brand systems and artifacts. It provides the visual workbench layer around deterministic Theme Forge components while keeping project state and evidence inspectable.

### Theme Forge Stellar Loom

**Repository:** [Knowledge-Forge-AI/theme-forge-stellar-loom](https://github.com/Knowledge-Forge-AI/theme-forge-stellar-loom)

Theme Forge Stellar Loom (TFSL) is a Starlight theme-builder backend, library, and CLI. It compiles typed, versioned theme specifications into deterministic CSS custom properties, theme descriptors, and installable Starlight theme packages, with validation and contrast diagnostics built into the workflow.

### Starlight Theme Terminal Nova

**Repository:** [Knowledge-Forge-AI/starlight-theme-terminal-nova](https://github.com/Knowledge-Forge-AI/starlight-theme-terminal-nova)

Starlight Theme Terminal Nova is an independent Starlight documentation theme generated with Theme Forge Stellar Loom. It serves both as a usable theme package and as a concrete public output of the Stellar Loom theme-generation pipeline.

### Knowledge Forge AI Website

**Repository:** [Knowledge-Forge-AI/Knowledge-Forge-AI.github.io](https://github.com/Knowledge-Forge-AI/Knowledge-Forge-AI.github.io)

Source for the Knowledge Forge AI public website and documentation presence, built with Astro and Starlight.

### Organization Community Health

**Repository:** [Knowledge-Forge-AI/.github](https://github.com/Knowledge-Forge-AI/.github)

Organization profile and default community-health files used by Knowledge Forge AI repositories that do not provide repository-local replacements.

## How the projects fit together

The public repositories are intentionally composable rather than one monolithic platform.

```text
Agent engineering
└── Agentic Praxis Grimoire

Theme Forge
├── Stellar Burst
│   └── deterministic SVG and asset lifecycle tooling
├── Stellar Loom
│   └── deterministic Starlight theme generation
├── Nebular Fusion
│   └── local visual workbench integrating Theme Forge capabilities
└── Starlight Theme Terminal Nova
    └── generated theme and reference output from Stellar Loom

Organization presence
├── Knowledge-Forge-AI.github.io
└── .github
    └── organization profile and default community-health policy
```

This separation keeps reusable engines, desktop tooling, generated artifacts, organization documentation, and community policy independently versioned and independently consumable.

## Project status

Knowledge Forge AI is actively developing these projects. Some repositories may represent release candidates, pre-release tooling, or components whose public packaging is still being qualified.

For authoritative project status, consult the repository README, release notes, tags, and published artifacts rather than assuming that every public repository is a stable release.

## Licensing model

Knowledge Forge AI generally uses the **GNU Affero General Public License v3.0 or later (`AGPL-3.0-or-later`)** as its community software license, with **separate commercial licensing** available where a repository says so.

The AGPL permits commercial use subject to its terms. A separate commercial license is an alternative for users who need proprietary or negotiated terms, which may include closed-source embedding, proprietary private SaaS modifications, OEM redistribution, proprietary product integration, support commitments, warranty or indemnity terms, or custom procurement and compliance terms.

Licensing is ultimately defined **per repository**. Always consult the applicable project's `LICENSE`, `NOTICE`, `COMMERCIAL-LICENSE.md`, third-party notices, and other licensing files before redistribution or integration. Repository-specific terms control if they differ from this organization-level summary.

For commercial licensing inquiries, contact **lair001@gmail.com**.

## Contributing

Knowledge Forge AI welcomes contributions under contribution terms designed to preserve both the AGPL community distribution and the ability to offer separate commercial licenses.

For repositories that do not provide their own contribution terms, the organization defaults are:

- [CONTRIBUTING.md](https://github.com/Knowledge-Forge-AI/.github/blob/main/CONTRIBUTING.md)
- [CLA.md](https://github.com/Knowledge-Forge-AI/.github/blob/main/CLA.md)

Contributors **retain copyright** in their contributions. By submitting a contribution under the applicable CLA, contributors grant **Samuel Leighton Lair, as project steward**, broad perpetual copyright and patent rights to use, modify, distribute, sublicense, and relicense the contribution as part of the applicable project, including under `AGPL-3.0-or-later`, commercial licenses, and future project licenses adopted by the project steward.

Contributions must be original work or submitted with authority from the relevant rights holder. Third-party code, documentation, generated material, or other content must be identified and may be submitted only when the contributor has the right to provide it under the applicable terms and all required notices are preserved.

For repositories using the organization-default CLA, each pull request must explicitly acknowledge:

```text
I agree to the Knowledge Forge AI contribution terms in CLA.md.
```

A `Signed-off-by` line does not replace that explicit acknowledgment. If a repository publishes its own `CLA.md`, `CONTRIBUTING.md`, or pull request template, **the repository-local terms and required acknowledgment control**.

---

**Website:** [knowledge-forge.ai](https://www.knowledge-forge.ai)  
**GitHub:** [Knowledge-Forge-AI](https://github.com/Knowledge-Forge-AI)
