# Richard Whitney

Director of Platform Automation. I build cloud platforms, and the tooling that lets AI agents work on them without burning context or bypassing controls.

[Writing (Medium)](https://medium.com/@rb1whitney) | [LinkedIn](https://www.linkedin.com/in/richard-whitney-0393b11a/)

[![ast-context-map tests](https://img.shields.io/github/actions/workflow/status/rb1whitney/ast-context-map/test.yml?branch=main&label=ast-context-map%20tests&style=flat-square)](https://github.com/rb1whitney/ast-context-map/actions/workflows/test.yml) [![vault_controller CI](https://img.shields.io/github/actions/workflow/status/rb1whitney/vault_controller/ci.yml?branch=main&label=vault_controller%20CI&style=flat-square)](https://github.com/rb1whitney/vault_controller/actions/workflows/ci.yml) [![cloud-boot-app CI](https://img.shields.io/github/actions/workflow/status/rb1whitney/cloud-boot-app/ci.yml?branch=master&label=cloud-boot-app%20CI&style=flat-square)](https://github.com/rb1whitney/cloud-boot-app/actions/workflows/ci.yml) [![factory lint](https://img.shields.io/github/actions/workflow/status/rb1whitney/agentic-project-factory/lint.yml?branch=master&label=factory%20lint&style=flat-square)](https://github.com/rb1whitney/agentic-project-factory/actions/workflows/lint.yml)
[![Targeted query savings](https://img.shields.io/badge/targeted_query_savings-97.6%25_on_sample-2ea043?style=flat-square)](https://github.com/rb1whitney/ast-context-map#measured) [![Medium articles](https://img.shields.io/badge/Medium_articles-4-12100E?style=flat-square&logo=medium&logoColor=white)](https://medium.com/@rb1whitney) [![PRs merged in own repos](https://img.shields.io/badge/PRs_merged_own_repos-84-8957e5?style=flat-square)](https://github.com/pulls?q=is%3Apr+author%3Arb1whitney+is%3Amerged)

## What I work on

Three themes. Each has an article that states the claim and code that shows it.

| Theme | Claim | Article | Code |
|---|---|---|---|
| Deterministic context for agents | Give an agent a structural map of the code (AST and graph), not raw files. | [Stop Dumping Raw Code into LLMs](https://medium.com/@rb1whitney/stop-dumping-raw-code-into-llms-why-semantic-graphs-lead-to-scalable-ai-agents-707c9c3220b0) | [ast-context-map](https://github.com/rb1whitney/ast-context-map) |
| Portable agents across harnesses | One canonical agent definition, compiled per harness. Harness defaults, not file formats, are the real portability risk. | [Taming Multi-Agent Workflows](https://medium.com/@rb1whitney/taming-multi-agent-workflows-7eec951375cf) | [agentic-project-factory](https://github.com/rb1whitney/agentic-project-factory) |
| Platform boundaries by responsibility | App teams declare what they need. The platform owns how it is built. | [One Platform Failed Our App Teams. The Other Failed Us.](https://medium.com/@rb1whitney/one-platform-failed-our-app-teams-the-other-failed-us-97cfcbd92f0b) | [cloud-boot-app](https://github.com/rb1whitney/cloud-boot-app) |
| Secrets as declared state | Vault configuration and secrets live in version control as Transit-encrypted YAML and are applied idempotently. | [Your Terraform Ports. Your Secrets Don't.](https://medium.com/@rb1whitney/your-terraform-ports-your-secrets-dont-2cff14cf4886) | [vault_controller](https://github.com/rb1whitney/vault_controller) |

## Repositories

| Repo | What it is |
|---|---|
| [ast-context-map](https://github.com/rb1whitney/ast-context-map) | Structural map of a codebase for coding agents: tree-sitter AST graph and queries, plus Kubernetes and Terraform topology graphs. Reproducible size benchmark and CI. |
| [agentic-project-factory](https://github.com/rb1whitney/agentic-project-factory) | Multi-agent swarm for infrastructure and cloud work. Skills, agent definitions, AST and graph tooling, and governance rules in one hub. |
| [nit-fabric](https://github.com/rb1whitney/nit-fabric) | Audits AWS and GCP connectivity: CIDR overlaps, VPC and BGP topology, security drift. Z3 solver for formal checks. |
| [cloud-boot-app](https://github.com/rb1whitney/cloud-boot-app) | Reference Java 21 / Spring Boot service on Kubernetes, managed with Terraform, Crossplane and Argo CD. |
| [vault_controller](https://github.com/rb1whitney/vault_controller) | Idempotent HashiCorp Vault state controller with built-in Transit Engine decryption for secure infrastructure as code. |

## In progress

Rewriting agent skills as a typed contract plus a concrete action template, then measuring tokens and LLM calls against the prose originals. Results and method will be published here with the code.

## Background

Nineteen years in infrastructure and site reliability; now directing platform automation teams.

- **Terraform Enterprise "Standard Environment":** consolidated 20+ repositories into a modular model and cut regional market launch time from 12 weeks to 2. Migrated 5,000+ Terraform states to enable cross-region provisioning.
- **Vault Enterprise:** globally dispersed high-availability clusters (talks below).
- **AI enablement:** CLI tooling and deterministic playbooks, 84% adoption across 400+ engineers.
- **Stack:** Python, Java, Go, Bash; GCP and AWS; Terraform, Vault, Kubernetes; Claude Code, Gemini CLI, Codex, Antigravity.
- **Certifications:** AWS Solutions Architect Associate (2018), AWS Developer Associate (2019), HashiCorp Terraform Associate and Vault Associate (2020).

## Talks

- [Vault is for everyone](https://youtu.be/K2HrZUC8UTY) (video)
- [Unlocking the Cloud Operating Model with Clover](https://www.hashicorp.com/en/events/webinars/unlocking-the-cloud-operating-model-with-clover) (HashiCorp webinar)

Related code: [vault_controller_example](https://github.com/rb1whitney/vault_controller_example) is the original shell version; [vault_controller](https://github.com/rb1whitney/vault_controller) is the current implementation.

## Writing

- Nov 2026: [Your Terraform Ports. Your Secrets Don't.](https://medium.com/@rb1whitney/your-terraform-ports-your-secrets-dont-2cff14cf4886)
- Oct 2026: [One Platform Failed Our App Teams. The Other Failed Us.](https://medium.com/@rb1whitney/one-platform-failed-our-app-teams-the-other-failed-us-97cfcbd92f0b)
- Sep 2026: [Taming Multi-Agent Workflows](https://medium.com/@rb1whitney/taming-multi-agent-workflows-7eec951375cf)
- Sep 2026: [Stop Dumping Raw Code into LLMs: Why ASTs lead to Scalable AI Agents](https://medium.com/@rb1whitney/stop-dumping-raw-code-into-llms-why-semantic-graphs-lead-to-scalable-ai-agents-707c9c3220b0)
