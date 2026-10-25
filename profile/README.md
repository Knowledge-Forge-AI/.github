# Knowledge Forge AI

Knowledge Forge AI builds deterministic, inspectable tools for agent engineering and human-reviewable software, design, and environment workflows.

Our public projects cover reusable coding-agent skills, repository intelligence, visual design systems, software distribution, declarative macOS workstations, and foundations for disposable test environments.

**[Join the community discussions](https://github.com/orgs/Knowledge-Forge-AI/discussions)** · **[Visit the website](https://www.knowledge-forge.ai)** · **[Browse all repositories](https://github.com/orgs/Knowledge-Forge-AI/repositories)**

> Project-specific READMEs, release notes, licenses, and contribution files are the source of truth for each repository's current maturity, compatibility, distribution, licensing, and contribution requirements.

## Contents

- [Community and feedback](#community-and-feedback)
- [Agent engineering and repository intelligence](#agent-engineering-and-repository-intelligence)
- [Theme Forge](#theme-forge)
- [Workstations and virtual-machine foundations](#workstations-and-virtual-machine-foundations)
- [Release and package distribution](#release-and-package-distribution)
- [Websites and community resources](#websites-and-community-resources)
- [How the projects fit together](#how-the-projects-fit-together)
- [Project status](#project-status)
- [Licensing model](#licensing-model)
- [Contributing](#contributing)

## Community and feedback

[Knowledge Forge AI Discussions](https://github.com/orgs/Knowledge-Forge-AI/discussions) is the shared forum for questions, ideas, first-use feedback, design conversations, and examples from across our public projects.

Tell us what you are trying to accomplish, where you got stuck, or what you would like to make easier. A short question, screenshot, workflow example, or account of your first few minutes with a tool can help improve the projects.

- **Ask and explore:** discuss a use case, propose an improvement, or ask how projects fit together.
- **Try and report:** share installation experiences, confusing instructions, or feedback on a particular release or preview.
- **Show and tell:** share a theme, documentation site, integration, or agent workflow.
- **Track concrete work:** use the relevant project's issue tracker for reproducible bugs and agreed improvements, and link related discussions.

Include the project name in your discussion title when it concerns a specific tool. Please follow our [Code of Conduct](https://github.com/Knowledge-Forge-AI/.github/blob/main/CODE_OF_CONDUCT.md) and the applicable repository's contribution guidance.

## Agent engineering and repository intelligence

| Project | Purpose |
| --- | --- |
| [**Agentic Praxis Grimoire (APGR)**](https://github.com/Knowledge-Forge-AI/agentic-praxis-grimoire) | A provider-neutral toolkit and skill corpus for bounded agent engineering. It provides task-scoped guidance, evidence capture, curated environment snapshots, structural repository analysis, context-footprint accounting, and a single-phase dispatcher for use by coding-agent platforms and harnesses. |
| [**RepoMap**](https://github.com/Knowledge-Forge-AI/repo-map) | A deterministic knowledge graph system for polyglot repositories. It connects entry points, scripts, imports, generated artifacts, tests, and environment contracts to source evidence, including behavior that crosses language boundaries. Its current reference distribution uses containerized PostgreSQL. |

APGR supplies reusable engineering primitives that callers compose into their own workflows. RepoMap develops repository intelligence with a documented Local, Server Engine, and Cloud product direction; SQLite Local, host-native MCP, and managed Cloud remain development targets.

## Theme Forge

Theme Forge separates reusable asset and theme engines, a desktop workbench, and independently distributed themes.

| Project | Purpose |
| --- | --- |
| [**Stellar Burst**](https://github.com/Knowledge-Forge-AI/theme-forge-stellar-burst) | A declarative SVG compiler and asset lifecycle toolkit. It converts a bounded SVG subset into editable TOML, produces deterministic SVG, installs assets into configured destinations, and detects or reconciles upstream and local changes. |
| [**Stellar Loom**](https://github.com/Knowledge-Forge-AI/theme-forge-stellar-loom) | A theme compiler, library, and CLI for Astro Starlight documentation sites. It produces CSS, theme descriptors, and installable theme packages from typed specifications, with contrast diagnostics and configurable documentation layouts. |
| [**Solar Sail**](https://github.com/Knowledge-Forge-AI/theme-forge-solar-sail) | A theme compiler, library, and CLI for Tailwind CSS v4 and shadcn/ui applications. It generates light and dark CSS tokens and standalone theme packages, complementing Stellar Loom's documentation focus. |
| [**Nebular Fusion**](https://github.com/Knowledge-Forge-AI/theme-forge-nebular-fusion) | A Tauri desktop workbench bringing together the Burst, Loom, and Solar engines for reviewing and managing brand systems and artifacts. Current source-build work targets Apple silicon macOS and Linux ARM64/AMD64; native builds and installed application behavior remain under qualification. |
| [**Starlight Theme Terminal Nova**](https://github.com/Knowledge-Forge-AI/starlight-theme-terminal-nova) | An independent Astro Starlight documentation theme built with Stellar Loom. It is both a concrete Theme Forge output and a theme package with its own presentation and distribution. |

See each project's README and release notes for supported inputs, integration details, and installation methods.

## Workstations and virtual-machine foundations

| Project | Purpose and current scope |
| --- | --- |
| [**Darwin Is Not a Snowflake (DINAS)**](https://github.com/Knowledge-Forge-AI/darwin-is-not-a-snowflake) | A modular macOS workstation framework built on nix-darwin. Core supplies bootstrap tooling, shared packages, configuration projection, and qualification and attended deployment machinery; domain adapters contribute through explicit contracts. The public preview targets Apple silicon macOS. |
| [**DINAS Composition**](https://github.com/Knowledge-Forge-AI/composition_dinas) | The composition layer assembling DINAS Core and an explicit registry of adapters, modules, overlays, commands, configuration, application ownership, and qualification checks. The public preview still references adapters whose source has not yet been published, so a public clone alone cannot build the full composition. |
| [**DINAS Browser UX**](https://github.com/Knowledge-Forge-AI/browser-ux_dinas) | An experimental DINAS adapter for declarative browser policies, browser-role and credential-provider contracts, convenience commands, and scrollbar presentation. Its public source preview requires a compatible nix-darwin composition; browser-extension packaging remains separate work. |
| [**Ephemeral Snowflake Artificer (ESA)**](https://github.com/Knowledge-Forge-AI/ephemeral-snowflake-artificer) | A foundation for reusable VM image seeds that consumers can clone into disposable job and test environments. The public implementation provides a versioned manifest and consumption contract, a Python validation CLI, and synthetic examples. NixOS and macOS image-building backends are planned. |

DINAS covers workstation configuration and composition. ESA develops a separate image contract and validation foundation; its current public source does not yet provide qualified VM images or an operational DINAS integration.

## Release and package distribution

| Repository | Role |
| --- | --- |
| [**Release Starport 9 (RS9)**](https://github.com/Knowledge-Forge-AI/release-starport-9) | Publication infrastructure under development to consume authoritative project releases, verify identity and provenance, and handle downstream packaging and publication. Projects remain responsible for their own source releases; supported publication routes are being qualified separately. |
| [**Theme Forge Packages**](https://github.com/Knowledge-Forge-AI/theme-forge-packages) | Distribution infrastructure and installation guidance for the Theme Forge family, including Nix, Arch/pacman, Fedora/RPM, and prepared AUR recipes. Check the repository and project releases for current availability and platform qualification. |
| [**Knowledge Forge AI Homebrew tap**](https://github.com/Knowledge-Forge-AI/homebrew-tap) | Homebrew formulae for Knowledge Forge AI tools, including APGR and Theme Forge. Available versions, installation methods, and supported platforms are documented per formula. |

These repositories serve different distribution roles. A planned RS9 destination does not establish that a package is available there; use the installation route documented for the specific project and release.

## Websites and community resources

| Repository | Role |
| --- | --- |
| [**Knowledge Forge AI website**](https://github.com/Knowledge-Forge-AI/Knowledge-Forge-AI.github.io) | Source for the public organization website and documentation presence, built with Astro and Starlight. |
| [**Sam Lair website**](https://github.com/Knowledge-Forge-AI/samlair.knowledge-forge.ai) | Astro and Starlight source for Sam Lair's personal site. |
| [**Organization profile and community resources**](https://github.com/Knowledge-Forge-AI/.github) | This organization profile and default community-health files. Join the shared forum through [organization Discussions](https://github.com/orgs/Knowledge-Forge-AI/discussions). Repository-local community files take precedence over applicable defaults. |

## How the projects fit together

| Area | Relationship |
| --- | --- |
| Agent engineering | APGR supplies reusable skills and deterministic workflow primitives; RepoMap develops source-grounded repository intelligence. Each can be evaluated and consumed on its own terms. |
| Design systems | Burst handles SVG assets, Loom handles Starlight themes, and Solar handles Tailwind/shadcn theme tokens. Nebular brings these engines into a desktop workbench; Terminal Nova is an independently distributed Loom-generated theme. |
| Workstation configuration | DINAS Core provides shared workstation machinery, Composition assembles adapters, and Browser UX is one domain adapter. |
| Disposable test environments | ESA is developing VM-image contracts and validation, with image-building backends still planned. |
| Distribution | Project releases remain authoritative. The Homebrew tap and Theme Forge Packages provide distribution surfaces, while RS9 develops shared downstream publication machinery. |

The repositories are independently versioned. Sharing an organization or a planned integration does not imply that every component is required to use every other component.

## Project status

Public work spans released components, early pilots, source previews, and foundations still under development. Availability and qualification can differ between operating systems, architectures, package managers, and releases.

For a usable starting point, consult the project's README, release notes, tags, and published artifacts. When reporting an experience in Discussions, include the project, version or source revision, and installation method so others can understand the result.

## Licensing model

Knowledge Forge AI generally uses the **GNU Affero General Public License v3.0 or later (`AGPL-3.0-or-later`)** as its community software license, with **separate commercial licensing** available where a repository says so.

The AGPL permits commercial use subject to its terms. A separate commercial license is an alternative for users who need proprietary or negotiated terms, which may include closed-source embedding, proprietary private SaaS modifications, OEM redistribution, proprietary product integration, support commitments, warranty or indemnity terms, or custom procurement and compliance terms.

Licensing is ultimately defined **per repository**. Always consult the applicable project's `LICENSE`, `NOTICE`, `COMMERCIAL-LICENSE.md`, third-party notices, and other licensing files before redistribution or integration. Repository-specific terms control if they differ from this organization-level summary.

For commercial licensing inquiries, contact **sam.lair@knowledge-forge.ai**.

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
**Discussions:** [Join the conversation](https://github.com/orgs/Knowledge-Forge-AI/discussions)
