# Power Platform Enterprise POC Projects (2026)

A portfolio of hands-on, enterprise-grade Proof-of-Concept projects covering the **entire Microsoft Power Platform stack** — Canvas Apps, Model-Driven Apps, Power Pages, Power Automate, AI Builder, and Copilot Studio (agents) — built on Microsoft Dataverse and SharePoint as data sources, and aligned to the **Power Platform 2026 Release Wave 1** capabilities (managed environments, real-time offline Dataverse, modern model-driven UI, multi-agent Copilot Studio orchestration, MCP tool integration, object-centric process mining, and AI-powered governance).

Each project is a standalone, demoable POC with its own architecture diagram, step-by-step build guide, and demo script. The final project is a **capstone** that unifies all six pillars into one coherent enterprise solution.

> **Author's note:** These projects are designed to reflect the kind of architectural decision-making (security modeling, ALM, governance, ROI measurement) expected from a senior/principal-level Power Platform practitioner — not just "how to drag a button onto a screen" tutorials.

---

## 📂 Projects

| # | Project | Pillar | Data Source | Details | Live Mockup |
|---|---|---|---|---|---|
| 1 | **FieldOps360** — Offline-first field service & inspection app | Canvas App | Dataverse + SharePoint | [View Project](./projects/01-canvas-field-ops/README.md) | [🔗 Preview](https://rahul7387.github.io/powerplatform-enterprise-poc-projects/projects/01-canvas-field-ops/index.html) |
| 2 | **CaseHub Enterprise** — IT/HR shared services case management | Model-Driven App | Dataverse | [View Project](./projects/02-model-driven-case-mgmt/README.md) | [🔗 Preview](https://rahul7387.github.io/powerplatform-enterprise-poc-projects/projects/02-model-driven-case-mgmt/index.html) |
| 3 | **VendorConnect** — External vendor self-service portal | Power Pages | Dataverse + SharePoint | [View Project](./projects/03-power-pages-vendor-portal/README.md) | [🔗 Preview](https://rahul7387.github.io/powerplatform-enterprise-poc-projects/projects/03-power-pages-vendor-portal/index.html) |
| 4 | **InvoiceFlow AP** — End-to-end accounts payable automation | Power Automate | SharePoint + Dataverse | [View Project](./projects/04-power-automate-invoice-ap/README.md) | [🔗 Preview](https://rahul7387.github.io/powerplatform-enterprise-poc-projects/projects/04-power-automate-invoice-ap/index.html) |
| 5 | **DocIntelligence** — Contract extraction, summarization & renewal-risk prediction | AI Builder | SharePoint + Dataverse | [View Project](./projects/05-ai-builder-doc-intelligence/README.md) | [🔗 Preview](https://rahul7387.github.io/powerplatform-enterprise-poc-projects/projects/05-ai-builder-doc-intelligence/index.html) |
| 6 | **ITHelpAgent** — Multi-agent IT helpdesk assistant | Copilot Studio | Dataverse + SharePoint | [View Project](./projects/06-copilot-studio-it-agent/README.md) | [🔗 Preview](https://rahul7387.github.io/powerplatform-enterprise-poc-projects/projects/06-copilot-studio-it-agent/index.html) |
| 7 | ⭐ **OnboardX360 (CAPSTONE)** — Full employee lifecycle platform using **all six pillars together** | All Pillars | Dataverse + SharePoint | [View Project](./projects/07-capstone-employee-lifecycle/README.md) | [🔗 Preview](https://rahul7387.github.io/powerplatform-enterprise-poc-projects/projects/07-capstone-employee-lifecycle/index.html) |

> Live mockups are static HTML/CSS pages approximating each product's real look & feel (Fluent UI styling, brand colors, layout conventions) — served via GitHub Pages. They are visual references only, not functional apps.

---

## 🧭 How to Use This Repo

- If you want to demo **one pillar at a time** to your manager or team, walk through Projects 1–6 individually — each is scoped to be built and demoed independently in a few days.
- If you want **one flagship project** that tells a complete story and proves platform-wide architectural maturity, go straight to **Project 7 (Capstone)** — it references the same design patterns used in Projects 1–6 but unifies them around one Dataverse-based employee lifecycle scenario.
- Every project README includes:
  - Business scenario & why it matters
  - A `mermaid` architecture diagram (renders natively on GitHub)
  - A numbered, phase-by-phase implementation plan
  - A demo script you can literally read from in a stakeholder meeting
  - A "skills this project proves" section, useful for performance reviews / portfolio conversations

---

## 🏗️ Common Architectural Principles Applied Across All Projects

These are the enterprise practices woven through every project in this repo — the details that separate a POC that impresses a manager from one that just "shows a screen":

1. **Solution-first development** — every component lives inside a Dataverse Solution from day one; nothing is built loose in the default environment.
2. **Environment strategy** — Dev / Test / Prod separation using **Managed Environments**, with DLP policies scoped per environment.
3. **Security modeling first, UI second** — Business Units, Security Roles, Field Security Profiles, and (for Power Pages) Web Roles/Table Permissions are designed before screens are built.
4. **Connection references & environment variables** — no hardcoded URLs/connections, enabling clean promotion across environments.
5. **ALM via Git** — solutions are version-controlled and promoted through pipelines (GitHub Actions/Azure DevOps), using the Power Platform's native GitHub-integrated ALM tooling introduced in 2026 Release Wave 1.
6. **Error handling & governance, not just happy-path demos** — try/catch flow patterns, exception logging, AI-powered governance agent monitoring, and human-in-the-loop review for low-confidence AI outputs.
7. **Measurable ROI** — each automation project includes a Power BI dashboard or metric (cycle time, containment rate, time-to-productivity) so business value is provable, not just implied.

---

## 🔧 Platform & Tooling Baseline (as of July 2026)

- **Power Platform 2026 Release Wave 1** (GA rollout April–September 2026)
- Dataverse with **real-time offline-first** access for Canvas Apps
- Model-driven apps using the **refreshed modern UI and standardized theming**
- Power Pages **AI-powered site generation** and **AI-powered security agent**
- Power Automate **self-healing flows**, **Copilot Studio-powered actions**, and **object-centric process mining**
- Copilot Studio **multi-agent orchestration**, **generative actions**, and **MCP-compliant tool integration**
- Power Platform admin center **AI-powered governance agents** for tenant-wide monitoring and remediation
- **GitHub-integrated ALM** ("Deploy from Git") for solution version control and pipeline-based promotion

---

## 📌 Suggested Presentation Order for Stakeholders

1. Start with the **Capstone (Project 7)** for the executive/manager audience — one coherent story, all pillars, clear ROI.
2. Use **Projects 1–6** as deep-dive appendices when a specific team (e.g., IT, Legal, Procurement) wants to see the pillar most relevant to them in more technical depth.

---

## 📄 License

This repository is provided as a personal learning/portfolio and internal proof-of-concept reference. Adapt freely for your own organization's POC needs.
