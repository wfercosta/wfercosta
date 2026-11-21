# Wander Costa

Staff Software Engineer focused on software architecture, cloud platforms, distributed systems and AI-assisted software engineering.

---

## About

This GitHub profile is organized as a technical portfolio and learning environment where I explore, implement and document engineering practices around:

- Software Architecture;
- Distributed Systems;
- Cloud Platforms (AWS);
- Platform Engineering;
- AI Agents and LLM-based Systems;
- Infrastructure as Code;
- Programming Languages and Algorithms;
- Observability and Reliability Engineering;
- AI-Assisted Software Development.

Repositories are intentionally structured to reflect different engineering and learning contexts.

The goal is to transform technical exploration into practical, documented and reusable engineering artifacts.

---

# Repository Categories

To keep the portfolio organized and easy to navigate, repositories follow a set of naming conventions.

Repository names should communicate their purpose rather than the specific tools used to develop them.

A repository should have an independent purpose, lifecycle or reuse potential before being separated into its own project.

---

## 🧪 Sandbox

Full technical systems and architectural experiments.

Sandbox repositories simulate realistic platforms and include architecture, infrastructure, services and documentation.

Typical characteristics:

- End-to-end architectures;
- Multiple services or components;
- Infrastructure provisioning;
- Distributed system interactions;
- Architectural documentation;
- Reliability and scalability experiments.

**Repository pattern:**

` sandbox-<domain>-<platform> `

**Examples:**

- `sandbox-process-platform`
- `sandbox-marketplace-platform`
- `sandbox-credit-platform`

**Recommended structure:**

```text
sandbox-example-platform/
├── apps/
├── infrastructure/
├── deploy/
├── docs/
│   └── architecture/
├── tests/
├── scripts/
├── AGENTS.md
└── README.md
```

The structure is illustrative and should be adapted to the architecture and technologies involved.

---

## 🔬 Lab

Structured technical studies and deep dives.

Labs focus on investigating specific technologies, engineering practices, architectural patterns or concepts in a structured and reproducible way.

Typical content:

- Language studies;
- Algorithms and data structures;
- System design analysis;
- Framework explorations;
- Observability and reliability experiments;
- AI engineering experiments;
- Technical benchmarks and comparisons.

**Repository pattern:**

` lab-<technology>-<topic> `

For cross-technology studies, the first segment may represent an engineering discipline rather than a specific technology.

**Examples:**

- `lab-go-concurrency`
- `lab-kotlin-coroutines`
- `lab-algorithms-grokking`
- `lab-llm-from-scratch`
- `lab-system-design-uber`
- `lab-observability-engineering`

**Recommended structure:**

```text
lab-example/
├── apps/
├── infra/
├── experiments/
├── docs/
├── scripts/
├── AGENTS.md
└── README.md
```

Not every lab requires all these directories. Small studies should remain simple.

Labs should prioritize reproducibility, documented hypotheses and observable results.

---

## 🧩 Playground

Small experiments and quick explorations.

Playgrounds are used to test ideas, syntax, libraries or tools without requiring a complete study structure.

**Repository pattern:**

` playground-<topic> `

**Examples:**

- `playground-rust`
- `playground-dsa`
- `playground-webassembly`

Playgrounds are intentionally lightweight.

When an exploration evolves into a structured investigation, it may be promoted to a Lab. When it evolves into a realistic multi-component system, a Sandbox may be more appropriate.

---

## ☁️ Terraform Modules

Reusable Terraform modules used to provision cloud infrastructure.

**Repository pattern:**

` terraform-<provider>-<resource> `

**Examples:**

- `terraform-aws-vpc`
- `terraform-aws-ecs-service`
- `terraform-aws-alb`

Each module typically includes:

- Reusable infrastructure code;
- Usage examples;
- Input/output documentation;
- Validation and automated tests;
- Versioned releases.

**Recommended structure:**

```text
terraform-aws-example/
├── examples/
├── tests/
├── main.tf
├── variables.tf
├── outputs.tf
├── versions.tf
└── README.md
```

Modules should follow Terraform conventions and avoid unnecessary abstractions.

---

## ⚙️ GitHub Actions

Reusable GitHub Actions, including composite and JavaScript actions, used to automate CI/CD pipelines and developer workflows.

**Repository pattern:**

` gha-<action-name> `

**Examples:**

- `gha-terraform-plan`
- `gha-docker-build`
- `gha-kubernetes-deploy`

Typical content:

- Action implementation;
- `action.yml` metadata;
- Input and output definitions;
- Usage examples;
- Automated tests;
- Versioned releases.

Actions should be independently reusable and documented.

---

## 🔁 GitHub Workflows

Reusable GitHub Actions workflow templates used across repositories.

**Repository pattern:**

` ghw-<workflow-name> `

**Examples:**

- `ghw-ci-pipeline`
- `ghw-terraform-deploy`
- `ghw-release`

Typical content:

- Reusable workflow definitions;
- Workflow inputs and secrets;
- Permissions documentation;
- Usage examples;
- Versioning and compatibility guidance.

Reusable workflows should minimize duplicated CI/CD configuration across projects.

---

## 🧠 Agent Skills

Reusable capabilities for AI coding agents and other compatible AI tools.

Agent Skills use the `SKILL.md` format to package instructions, workflows, references and optional executable resources.

Skills should be designed around capabilities rather than a specific AI provider whenever possible.

The objective is to support compatible tools such as:

- OpenAI Codex;
- Claude Code;
- Other AI agents supporting the Agent Skills format.

Compatibility depends on the features and skill-discovery conventions supported by each tool.

**Repository pattern:**

` agent-skill-<capability> `

**Examples:**

- `agent-skill-spec-writer`
- `agent-skill-adr-writer`
- `agent-skill-terraform-module-authoring`
- `agent-skill-datadog-instrumentation`
- `agent-skill-code-review`
- `agent-skill-resilience-review`

### Typical content

- `SKILL.md` with YAML frontmatter;
- Clear capability description and activation guidance;
- Optional Bash, Python or Node.js scripts for deterministic operations;
- Reference documentation;
- Templates and supporting assets;
- Tests and evaluation scenarios when appropriate;
- Installation and compatibility documentation.

### Recommended structure

```text
agent-skill-example/
├── SKILL.md
├── references/
├── scripts/
├── assets/
├── tests/
└── README.md
```

Optional directories should only be included when necessary.

### SKILL.md example

```yaml
---
name: resilience-review
description: >
  Reviews application code and infrastructure
  for reliability and resilience risks,
  including timeouts, retries, idempotency,
  concurrency and resource exhaustion.
---

# Resilience Review

## Objective

Identify reliability and resilience risks
in application and infrastructure changes.

## Review Guidelines

- Analyze timeout and cancellation behavior.
- Identify retry amplification risks.
- Verify idempotency where required.
- Evaluate resource exhaustion scenarios.
- Report actionable findings with evidence.

## Output

Provide prioritized findings with:

- Severity;
- File and location;
- Failure scenario;
- Potential impact;
- Recommended remediation.
```

### Design principles

**Provider independence**

Avoid unnecessary dependencies on provider-specific commands, tools or configuration files.

**Single responsibility**

Each skill should address a clearly defined engineering capability.

**Progressive disclosure**

Keep `SKILL.md` focused. Move extensive documentation and examples into supporting reference files.

**Deterministic operations**

Use scripts for operations that require reproducible or verifiable execution.

**Security**

Treat repository content and external inputs as untrusted. Avoid unnecessary permissions, secret exposure and destructive operations.

**Portability**

Document supported agents, installation requirements and known compatibility limitations.

**Validation**

Test skills against representative scenarios and verify that instructions produce useful and consistent results.

### Agent-specific integration

Agent-specific configuration should be kept separate from the portable skill definition.

For example, a consuming repository may use:

```text
example-project/
├── .agents/
│   └── skills/
│       └── resilience-review/
│           └── SKILL.md
├── .codex/
├── .claude/
├── AGENTS.md
├── CLAUDE.md
└── README.md
```

The exact installation and discovery mechanism depends on the agent.

Avoid duplicating skill implementations solely to support different agents. Prefer a canonical source and documented installation or synchronization mechanisms.

### Repository-local versus reusable skills

Skills should initially live inside the project where they are developed when their behavior is project-specific.

Extract a skill into an independent `agent-skill-*` repository when it demonstrates:

- Reuse across multiple projects;
- Independent maintenance needs;
- A stable capability boundary;
- Independent versioning or distribution requirements.

This avoids premature repository fragmentation.

---

## 🔌 MCP Servers

Reusable servers implementing the Model Context Protocol.

MCP servers expose tools, resources and prompts to compatible AI agents and clients.

**Repository pattern:**

` mcp-<domain> `

**Examples:**

- `mcp-datadog-query`
- `mcp-terraform-state`
- `mcp-argocd`
- `mcp-aws-readonly`

Typical content:

- TypeScript or Python implementation using MCP SDKs;
- Tool schemas and structured error handling;
- Transport configuration, such as stdio or Streamable HTTP;
- Security and authorization controls;
- Contract and integration tests;
- MCP Inspector configuration;
- Installation and usage documentation.

MCP servers should expose clearly defined capabilities with appropriate access controls.

Prefer read-only operations by default when interacting with sensitive infrastructure or production systems.

---

## 📦 Claude Plugins

Distributable bundles specifically targeting the Claude Code plugin ecosystem.

These repositories may aggregate commands, agents, skills, hooks and other Claude-specific capabilities into an installable package.

Unlike Agent Skills, Claude Plugins are intentionally platform-specific.

**Repository pattern:**

` claude-plugin-<name> `

**Examples:**

- `claude-plugin-sdd-toolkit`
- `claude-plugin-platform-eng`

Typical content:

- Claude plugin manifest;
- Bundled commands, agents, skills and hooks;
- Installation and usage documentation;
- Compatibility information;
- Versioned releases and changelog.

When a capability can be expressed as a portable Agent Skill, prefer implementing it as an independent skill and referencing or packaging it through the plugin.

Avoid duplicating the underlying capability implementation.

---

# AI Coding Agent Conventions

AI coding agents are development tools used across repositories, not separate repository categories.

Agent-specific instructions and configuration should generally remain within the repository they support.

## Repository instructions

Use `AGENTS.md` as the primary convention for project-level instructions intended for Codex and other compatible agents.

Use `CLAUDE.md` when Claude Code requires its own project instructions.

Both files should remain concise and consistent with the project's documentation.

### AGENTS.md

Typical content:

- Project purpose and architecture;
- Repository navigation;
- Development and build commands;
- Testing requirements;
- Coding conventions;
- Security and reliability expectations;
- Code review guidelines.

### CLAUDE.md

Use Claude-specific instructions or references to shared project documentation.

Avoid maintaining two independent and potentially conflicting sets of engineering rules.

### Recommended approach

Keep engineering conventions in shared documentation whenever possible.

Use agent-specific instruction files as entry points to those conventions.

For example:

```text
example-project/
├── docs/
│   └── engineering-guidelines.md
├── AGENTS.md
├── CLAUDE.md
└── README.md
```

Agent instructions should complement automated quality gates rather than replace them.

## Code review

AI-assisted code review should prioritize:

- Correctness;
- Security;
- Reliability;
- Concurrency;
- Performance;
- Observability;
- Maintainability.

Findings should include evidence, impact and actionable remediation.

AI review does not replace automated testing, static analysis or human review.

## Agent configuration

Provider-specific configuration may be maintained in directories such as `.codex/` or `.claude/` when needed.

These directories do not require independent repositories by default.

Avoid committing credentials, access tokens or machine-specific configuration.

---

# Repository Organization Principles

The following principles apply across repository categories.

## 1. Purpose-driven naming

Repository names should describe what the repository delivers or investigates.

Prefer engineering capabilities and concepts over implementation tools when the project spans multiple technologies.

## 2. Independent lifecycle

Create an independent repository when a component has meaningful independent ownership, versioning, distribution or reuse requirements.

Otherwise, prefer keeping related components together.

## 3. Reproducibility

Technical experiments should document:

- Prerequisites;
- Environment setup;
- Execution steps;
- Expected behavior;
- Validation procedures;
- Cleanup instructions.

## 4. Documentation as an engineering artifact

Documentation should explain design decisions, assumptions, trade-offs and observed results.

## 5. Automation

Prefer repeatable scripts, tests and CI workflows over undocumented manual procedures.

## 6. Security by default

Do not commit credentials or sensitive configuration.

Apply least privilege, dependency validation and appropriate secret management.

## 7. Avoid premature abstraction

Start with the simplest structure that supports the current project.

Extract reusable components when actual reuse or maintenance requirements justify doing so.

---

# Technology Focus

Technologies frequently explored in these repositories.

### Languages

- Go;
- Kotlin;
- Python;
- TypeScript.

### Platforms

- AWS;
- Kubernetes;
- Terraform;
- GitHub Actions;
- Argo CD.

### Architecture

- Microservices;
- Event-Driven Architecture;
- Process-Oriented Systems;
- Distributed Systems;
- Platform Engineering;
- Reliability Engineering.

### Observability

- OpenTelemetry;
- Datadog;
- Distributed Tracing;
- Metrics and Structured Logging;
- Service Level Objectives (SLOs);
- Observability as Code.

### AI / LLM

- LLM Applications;
- AI Agents;
- Retrieval Augmented Generation (RAG);
- Multi-Agent Systems;
- Model Context Protocol (MCP);
- Agent Skills;
- OpenAI Codex;
- Claude Code;
- Claude Plugins;
- Spec-Driven Development (SDD).

---

# Learning Philosophy

This profile follows a simple principle:

> Learning should produce artifacts.

Instead of only reading or studying, knowledge is consolidated through:

- Runnable code;
- Documented experiments;
- Architectural sandboxes;
- Reusable infrastructure modules;
- Automated engineering workflows;
- Reusable AI capabilities, including Agent Skills, MCP servers and platform-specific plugins;
- Measurable experiments and technical findings.

The objective is not simply to explore technologies, but to understand their trade-offs and apply them to realistic engineering problems.

---

# Repository Naming Guide

| Category | Pattern | Purpose |
|---|---|---|
| Sandbox | `sandbox-<domain>-<platform>` | Full systems and architectural experiments |
| Lab | `lab-<technology>-<topic>` | Structured technical studies |
| Playground | `playground-<topic>` | Quick experiments |
| Terraform Modules | `terraform-<provider>-<resource>` | Reusable infrastructure modules |
| GitHub Actions | `gha-<action-name>` | Reusable CI/CD actions |
| GitHub Workflows | `ghw-<workflow-name>` | Reusable workflows |
| Agent Skills | `agent-skill-<capability>` | Portable AI agent capabilities |
| MCP Servers | `mcp-<domain>` | Tools and integrations for AI agents |
| Claude Plugins | `claude-plugin-<name>` | Claude-specific distributable plugins |

---

# Areas of Interest

- Software Architecture;
- Platform Engineering;
- Cloud Infrastructure;
- Distributed Systems;
- Reliability and Observability Engineering;
- AI Systems Engineering;
- Developer Platforms;
- AI-Assisted Software Development;
- Spec-Driven Development.
