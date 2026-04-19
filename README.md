# Wander Costa

Staff Software Engineer focused on software architecture, cloud
platforms and engineering distributed systems.

---

## About

This GitHub profile is organized as a **technical portfolio and learning
environment** where I explore and document engineering practices around:

- Software Architecture;
- Distributed Systems;
- Cloud Platforms (AWS);
- Platform Engineering;
- AI Agents and LLM-based systems;
- Infrastructure as Code;
- Programming Languages and Algorithms

Repositories are intentionally structured to reflect **different
engineering and learning contexts**.

---

# Repository Categories

To keep the portfolio organized and easy to navigate, repositories
follow a set of naming conventions.

---

## 🧪 Sandbox

**Full technical systems and architectural experiments.**

Sandbox repositories simulate realistic platforms and include
architecture, infrastructure, services and documentation.

Typical characteristics:

- End-to-end architectures;
- Multiple services or components;
- Infrastructure provisioning;
- Architectural documentation

Repository pattern:

```
sandbox-<domain>-<platform>
```

Examples:

`sandbox-process-platform` · `sandbox-marketplace-platform` · `sandbox-credit-platform`

---

## 🔬 Lab

**Structured technical studies and deep dives.**

Labs focus on investigating specific technologies, patterns or concepts
in a structured way.

Typical content:

- Language studies;
- Algorithms and data structures;
- System design analysis;
- Framework explorations;
- Technical experiments

Repository pattern:

```
lab-<technology>-<topic>
```

Examples:

`lab-go-concurrency` · `lab-kotlin-coroutines` · `lab-algorithms-grokking` · `lab-llm-from-scratch` · `lab-system-design-uber`

---

## 🧩 Playground

**Small experiments and quick explorations.**

Playgrounds are used to test ideas, syntax or libraries quickly.

Repository pattern:

```
playground-<topic>
```

Examples:

`playground-rust` · `playground-dsa` · `playground-webassembly`

---

## ☁️ Terraform Modules

Reusable Terraform modules used to provision cloud infrastructure.

Repository pattern:

```
terraform-<provider>-<resource>
```

Examples:

`terraform-aws-vpc` · `terraform-aws-ecs-service` · `terraform-aws-alb`

Each module typically includes:

- Reusable infrastructure code;
- Usage examples;
- Input/output documentation;
- Versioned releases

---

## ⚙️ GitHub Actions

Reusable GitHub Actions (composite and JavaScript) used to automate
CI/CD pipelines.

Repository pattern:

```
gha-<action-name>
```

Examples:

`gha-terraform-plan` · `gha-docker-build` · `gha-kubernetes-deploy`

---

## 🔁 GitHub Workflows

Reusable workflow templates used across repositories.

Repository pattern:

```
ghw-<workflow-name>
```

Examples:

`ghw-ci-pipeline` · `ghw-terraform-deploy` · `ghw-release`

---

## 🧠 Claude Code Skills

Reusable skills in the Anthropic `SKILL.md` format — auto-triggered by
description and consumable by Claude Code, Claude apps, and any tool
that supports the format.

Typical content:

- `SKILL.md` with frontmatter and engineered description;
- Optional capability scripts (Bash/Python/Node) for deterministic steps;
- Templates, reference files, and assets used during execution;
- Evaluation suite validating activation and behavior

Repository pattern:

```
claude-skill-<capability>
```

Examples:

`claude-skill-spec-writer` · `claude-skill-adr-writer` · `claude-skill-terraform-module-authoring` · `claude-skill-datadog-instrumentation`

---

## 🔌 MCP Servers

Reusable servers implementing the **Model Context Protocol** — exposing
tools, resources and prompts to AI agents and clients that speak MCP
(Claude Code, Claude Desktop, editors, custom agents).

Typical content:

- TypeScript or Python implementation using the official MCP SDKs;
- Tool schemas and typed errors;
- Transport configuration (stdio and/or HTTP/SSE);
- Security and authorization layer;
- Contract tests and MCP Inspector configuration

Repository pattern:

```
mcp-<domain>
```

Examples:

`mcp-datadog-query` · `mcp-terraform-state` · `mcp-argocd` · `mcp-aws-readonly`

---

## 📦 Claude Plugins

Distributable bundles that aggregate **commands, subagents, skills and
hooks** into a single installable unit — typically consumed via a
Claude Code marketplace.

Typical content:

- `plugin.json` manifest;
- Bundled slash commands, subagents, skills and hooks;
- Installation and usage documentation;
- Versioned releases and changelog

Repository pattern:

```
claude-plugin-<name>
```

Examples:

`claude-plugin-sdd-toolkit` · `claude-plugin-platform-eng`

---

# Technology Focus

Technologies frequently explored in these repositories.

### Languages

- Go;
- Kotlin;
- Python;
- TypeScript

### Platforms

- AWS;
- Kubernetes;
- Terraform;
- GitHub Actions;
- Argo CD

### Architecture

- Microservices;
- Event-Driven Architecture;
- Process-Oriented Systems;
- Platform Engineering

### AI / LLM

- LLM applications;
- AI agents;
- Retrieval Augmented Generation (RAG);
- Multi-agent systems;
- Model Context Protocol (MCP);
- Claude Code skills and plugins;
- Spec Driven Development (SDD)

---

# Learning Philosophy

This profile follows a simple principle:

> Learning should produce artifacts.

Instead of only reading or studying, knowledge is consolidated through:

- Runnable code;
- Documented experiments;
- Architectural sandboxes;
- Reusable infrastructure modules;
- Reusable AI capabilities (skills, MCP servers, plugins)

---

# Repository Naming Guide

| Category | Pattern |
| --- | --- |
| Sandbox | `sandbox-*` |
| Lab | `lab-*` |
| Playground | `playground-*` |
| Terraform Modules | `terraform-*` |
| GitHub Actions | `gha-*` |
| GitHub Workflows | `ghw-*` |
| Claude Code Skills | `claude-skill-*` |
| MCP Servers | `mcp-*` |
| Claude Plugins | `claude-plugin-*` |

---

# Areas of Interest

- Software Architecture;
- Platform Engineering;
- Cloud Infrastructure;
- Distributed Systems;
- AI Systems Engineering;
- Developer Platforms;
- Spec Driven Development
