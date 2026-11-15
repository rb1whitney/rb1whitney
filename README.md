# Richard Whitney

Director of Platform Automation. I build cloud platforms, and the tooling that lets AI agents work on them without burning context or bypassing controls.

[Writing (Medium)](https://medium.com/@rb1whitney) | [LinkedIn](https://www.linkedin.com/in/richard-whitney-0393b11a/)

[![ast-context-map tests](https://img.shields.io/github/actions/workflow/status/rb1whitney/ast-context-map/test.yml?branch=main&label=ast-context-map%20tests&style=flat-square)](https://github.com/rb1whitney/ast-context-map/actions/workflows/test.yml) [![vault_controller CI](https://img.shields.io/github/actions/workflow/status/rb1whitney/vault_controller/ci.yml?branch=main&label=vault_controller%20CI&style=flat-square)](https://github.com/rb1whitney/vault_controller/actions/workflows/ci.yml) [![cloud-boot-app CI](https://img.shields.io/github/actions/workflow/status/rb1whitney/cloud-boot-app/ci.yml?branch=master&label=cloud-boot-app%20CI&style=flat-square)](https://github.com/rb1whitney/cloud-boot-app/actions/workflows/ci.yml) [![factory lint](https://img.shields.io/github/actions/workflow/status/rb1whitney/agentic-project-factory/lint.yml?branch=master&label=factory%20lint&style=flat-square)](https://github.com/rb1whitney/agentic-project-factory/actions/workflows/lint.yml)
[![Research](https://img.shields.io/badge/research-18_findings,_115_runs-2ea043?style=flat-square)](https://github.com/rb1whitney/ast-context-map/blob/main/research/graph-of-graphs/FINDINGS.md) [![Medium articles](https://img.shields.io/badge/Medium_articles-4-12100E?style=flat-square&logo=medium&logoColor=white)](https://medium.com/@rb1whitney) [![PRs merged in own repos](https://img.shields.io/badge/PRs_merged_own_repos-84-8957e5?style=flat-square)](https://github.com/pulls?q=is%3Apr+author%3Arb1whitney+is%3Amerged)

## What I work on

Four themes. Each has an article that states the claim and code that shows it.

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

## Current research

Do semantic code graphs help coding agents, or does plain search win? I measured it on public repositories with a small model (115 agent runs, $1.15 in total).

- Search was cheaper than the first graph tool, which needed 36 turns against 20.
- A single `closure` query with a coverage footer cost $0.004 per run against $0.013 for search, at F1 0.84 against 0.94.
- Agents answered from the graph and rarely verified, so an unverified graph answer is a risk.

Method, answer keys, limits and what not to claim: [FINDINGS.md](https://github.com/rb1whitney/ast-context-map/blob/main/research/graph-of-graphs/FINDINGS.md).

## Talks

- [Vault is for everyone](https://youtu.be/K2HrZUC8UTY) (video)
- [Unlocking the Cloud Operating Model with Clover](https://www.hashicorp.com/en/events/webinars/unlocking-the-cloud-operating-model-with-clover) (HashiCorp webinar)

Related code: [vault_controller_example](https://github.com/rb1whitney/vault_controller_example) is the original shell version; [vault_controller](https://github.com/rb1whitney/vault_controller) is the current implementation.
