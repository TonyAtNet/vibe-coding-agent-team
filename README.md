# Vibe Coding Agent Team

<div align="center">

<p align="center">
  <strong>21 AI-Native Role Configurations for AI IDEs</strong><br>
  Directly import into Cursor / Claude Code / Kimi Code / Trae and use immediately
</p>

<p align="center">
  <a href="LICENSE"><img src="https://img.shields.io/badge/License-MIT-yellow.svg" alt="License: MIT"></a>
  <img src="https://img.shields.io/badge/Agents-21-blue.svg" alt="Agents: 21">
  <img src="https://img.shields.io/badge/Vibe%20Coding-AI%20Native-green.svg" alt="Vibe Coding: AI Native">
  <a href="zh-CN/README.md"><img src="https://img.shields.io/badge/中文文档-README-red.svg" alt="中文文档"></a>
</p>

<p align="center">
  <a href="#quick-start">Quick Start</a> ·
  <a href="#project-structure">Project Structure</a> ·
  <a href="#usage-example">Usage Example</a> ·
  <a href="#contribution-guide">Contribution Guide</a> ·
  <a href="zh-CN/README.md">中文文档</a> ·
  <a href="#license">License</a>
</p>

</div>

---

## Project Introduction

Vibe Coding Agent Team is a set of **AI-Native agent role configurations** for the **Vibe Coding era**, containing **21 professional roles** covering the complete chain from trend research, product definition, prototype validation to development, testing, deployment, and operations.

Each role file contains:
- Complete System Prompt configuration (directly importable into AI IDEs)
- Executable spec templates (not static documents, directly consumable by AI)
- Standardized workflows (step-by-step operation guides)
- Success metrics and AI observability metrics
- Modern toolchain declarations (Cursor, v0, Lovable, MCP, LangChain, etc.)

### Core Design Principles

| Principle | Description |
|-----------|-------------|
| **Zero Emoji** | All files contain no emoji, maintaining professionalism |
| **Zero Role-Playing** | Remove "You are Alex", "10 years experience" and other false personas; define identity by capability |
| **Executable Specs** | Deliverables are prompt templates and code configurations that AI IDEs can directly execute, not static documents |
| **RICE-V Scoring** | Introduce Vibe Speed and Model Risk assessment for data-driven priority decisions |
| **AI Observability** | Every role includes hallucination rate, TTFT, token cost, human-in-the-loop rate |

---

## Quick Start

### 1. Select a Role

Choose the corresponding role file based on your current project stage:

```
Project Initiation    →  vibe-trend-researcher + vibe-prototyper
Product Definition    →  product-manager + vibe-behavioral-designer
Technical Architecture →  vibe-architect + vibe-priority-orchestrator
Development Phase     →  vibe-frontend-engineer / vibe-backend-engineer / vibe-mobile-engineer + vibe-ai-llm-engineer
Quality Assurance     →  vibe-qa-automation-engineer + vibe-code-reviewer + vibe-security-engineer
Deployment & Ops      →  vibe-devops-engineer + vibe-database-engineer + vibe-data-engineer
Documentation         →  vibe-tech-writer
Team Expansion      →  vibe-onboarding-engineer
Feedback Iteration    →  vibe-feedback-analyst
```

### 2. Import into AI IDE

**Cursor**:
1. Open Cursor Settings → Rules
2. Create a new Rule, paste the `.md` file content into the System Prompt
3. Save and @mention the role in conversations to invoke it

**Claude Code**:
1. Create `CLAUDE.md` in the project root
2. Append the role file content to `CLAUDE.md`
3. Automatically loads when running `claude`

**Kimi Code / Trae / Roo Code**:
Import the `.md` file content as System Prompt or role configuration.

### 3. Start Collaboration

Each role file contains a complete workflow. For example, invoking `vibe-prototyper`:

> "Please follow your workflow and help me turn this requirement into an interactive prototype. The requirement is: an AI-driven todo app where users can add tasks using natural language."

The role will automatically execute: requirement understanding → AI prototype generation → user testing design → insight analysis → prototype-to-code migration.

---

## Project Structure

```
vibe-coding-agent-team/
├── LICENSE                              # MIT License
├── README.md                            # English (this file)
├── zh-CN/README.md                      # Chinese version
│
├── product/                             # Product-side roles (5) — Chinese
│   ├── product-manager.md
│   ├── vibe-behavioral-designer.md
│   ├── vibe-feedback-analyst.md
│   ├── vibe-priority-orchestrator.md
│   └── vibe-trend-researcher.md
│
├── engineering/                         # Engineering-side roles (16) — Chinese
│   ├── vibe-ai-llm-engineer.md
│   ├── vibe-architect.md
│   ├── vibe-backend-engineer.md
│   ├── vibe-code-reviewer.md
│   ├── vibe-database-engineer.md
│   ├── vibe-data-engineer.md
│   ├── vibe-devops-engineer.md
│   ├── vibe-frontend-engineer.md
│   ├── vibe-git-master.md
│   ├── vibe-minimal-change-engineer.md
│   ├── vibe-mobile-engineer.md
│   ├── vibe-onboarding-engineer.md
│   ├── vibe-prototyper.md
│   ├── vibe-qa-automation-engineer.md
│   ├── vibe-security-engineer.md
│   └── vibe-tech-writer.md
│
├── zh-CN/                               # Chinese versions
│   ├── product/                           # Chinese product roles (5)
│   └── engineering/                       # Chinese engineering roles (16)
│
├── en/                                  # English versions
│   ├── product/                           # English product roles (5)
│   └── engineering/                       # English engineering roles (16)
│
├── examples/                            # Example projects
│   └── ai-note-assistant/                 # End-to-end example (8 stages)
│
├── scripts/                             # Build and validation scripts
│   ├── validate.py
│   └── build-site.py
│
└── docs/                                # GitHub Pages site
    └── index.html
```

**Total: 21 agent roles (Chinese + English bilingual)**

---

## Usage Example

### Scenario: Quickly Validate a Product Hypothesis

```
Step 1: Invoke vibe-trend-researcher
  "Research 2026 AI todo app market trends, output executable trend spec"

Step 2: Invoke vibe-prototyper
  "Based on the trend spec, use v0 to generate an interactive prototype, target: complete within 2 hours"

Step 3: Invoke vibe-priority-orchestrator
  "RICE-V score the prototype validation results, decide whether to proceed to development"

Step 4: Invoke product-manager + vibe-behavioral-designer
  "Output executable product spec, including design tokens and component specifications"

Step 5: Invoke vibe-architect + vibe-frontend-engineer + vibe-backend-engineer
  "Develop according to spec, using Cursor for AI-assisted coding"

Step 6: Invoke vibe-qa-automation-engineer + vibe-code-reviewer
  "Automated testing + code review + security scanning"

Step 7: Invoke vibe-devops-engineer
  "Deploy to Vercel, configure observability"

Step 8: Invoke vibe-tech-writer
  "Synchronously update documentation, ensure code and docs are consistent"
```

---

## Role Capability Quick Reference

| Role | Core Capability | Key Toolchain | Vibe Speed |
|------|--------------|-------------|------------|
| vibe-trend-researcher | AI-driven trend research | Perplexity, Deep Research, Kimi Research | Days |
| vibe-prototyper | Hours-level prototype validation | v0, Lovable, Bolt, Cursor | Hours |
| vibe-priority-orchestrator | RICE-V dynamic priority | PostHog, Amplitude, Langfuse | Days |
| vibe-behavioral-designer | Agent experience design | System Prompt engineering, MCP tool design | Days |
| vibe-feedback-analyst | LLM semantic feedback analysis | Vector databases, RAG pipelines | Days |
| vibe-architect | MCP ecosystem architecture | Terraform, Kubernetes, Vercel | Weeks |
| vibe-ai-llm-engineer | LLM application development | LangChain, Vercel AI SDK, Langfuse | Days |
| vibe-frontend-engineer | AI-assisted frontend development | Cursor, v0 Dev Mode, Tailwind | Days |
| vibe-backend-engineer | AI-assisted backend development | Cursor, Claude Code, Supabase | Days |
| vibe-qa-automation-engineer | AI-driven quality gates | Intelligent test generation, visual regression, security scanning | Days |
| vibe-security-engineer | AI security audit | Prompt injection detection, zero-trust architecture | Days |
| vibe-devops-engineer | AI deployment & observability | Terraform, Kubernetes, Helicone | Days |
| vibe-database-engineer | Database design & optimization | Supabase, Pinecone, Qdrant | Days |
| vibe-data-engineer | Data pipelines & RAG | ETL, vector databases, data quality | Weeks |
| vibe-git-master | AI-era Git workflow | Conventional Commits, automated merging | Hours |
| vibe-onboarding-engineer | New hire Day 1 onboarding | Dev Containers, AI-assisted onboarding | Days |
| vibe-tech-writer | Living documentation & knowledge base | Docs-as-code, runnable examples | Days |
| vibe-code-reviewer | AI code review | Code quality, security vulnerabilities, performance | Hours |
| vibe-mobile-engineer | AI mobile development | Cursor, React Native, Flutter | Days |
| vibe-minimal-change-engineer | Surgical changes | Minimal change principle, impact assessment | Hours |
| product-manager | Product definition & decisions | RICE-V, executable specs | Days |

---

## Contribution Guide

We welcome all contributions! Whether it is:
- New roles
- Improving existing role prompts or workflows
- Correcting toolchains or links
- Adding usage examples
- Translations

### Before Submitting Checklist

- [ ] File uses YAML Frontmatter, containing `name`, `description`, `color` fields
- [ ] File content contains no emoji
- [ ] Contains no false role-playing ("You are Alex", "10 years experience", etc.)
- [ ] Contains all required sections (core mission, key principles, technical deliverables, workflow, success metrics, communication style)
- [ ] Contains modern AI toolchain declarations
- [ ] Contains AI observability metrics (hallucination rate, TTFT, token cost)
- [ ] Local validation passes: `python scripts/validate.py` with no errors

### How to Submit

1. Fork this repository
2. Create your branch (`git checkout -b feature/new-role`)
3. Submit changes (`git commit -am 'Add vibe-xxx role'`)
4. Push to branch (`git push origin feature/new-role`)
5. Create Pull Request

See [CONTRIBUTING.md](CONTRIBUTING.md) for details.

---

## License

This project is open-sourced under the [MIT License](LICENSE).

You are free to use, modify, and distribute, including for commercial purposes. Just retain the original copyright notice.

---

## Acknowledgments

This project's role design is inspired by the latest practices in the Vibe Coding ecosystem, including usage experience with Cursor, v0, Lovable, Claude Code, Kimi Code, and other AI tools, as well as cutting-edge methodologies like the MCP protocol and RICE-V scoring framework.

Special thanks to all contributors and users for their feedback, which allows this agent team to continuously evolve.

---

<div align="center">

**Build Vibe products with AI teams.**

</div>
