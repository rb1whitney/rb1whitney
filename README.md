# Richard Whitney

Director of Platform Automation. I build cloud platforms, and the tooling that lets AI agents work on them without burning context or bypassing controls.

[Writing (Medium)](https://medium.com/@rb1whitney) | [LinkedIn](https://www.linkedin.com/in/richard-whitney-0393b11a/)

## What I work on

Three themes. Each has an article that states the claim and code that shows it.

| Theme | Claim | Article | Code |
|---|---|---|---|
| Deterministic context for agents | Give an agent a structural map of the code (AST and graph), not raw files. | [Stop Dumping Raw Code into LLMs](https://medium.com/@rb1whitney/stop-dumping-raw-code-into-llms-why-semantic-graphs-lead-to-scalable-ai-agents-707c9c3220b0) | [agentic-project-factory](https://github.com/rb1whitney/agentic-project-factory) |
| Portable agents across harnesses | One canonical agent definition, compiled per harness. Harness defaults, not file formats, are the real portability risk. | [Taming Multi-Agent Workflows](https://medium.com/@rb1whitney/taming-multi-agent-workflows-7eec951375cf) | [agentic-project-factory](https://github.com/rb1whitney/agentic-project-factory) |
| Platform boundaries by responsibility | App teams declare what they need. The platform owns how it is built. | [One Platform Failed Our App Teams. The Other Failed Us.](https://medium.com/@rb1whitney/one-platform-failed-our-app-teams-the-other-failed-us-97cfcbd92f0b) | [cloud-boot-app](https://github.com/rb1whitney/cloud-boot-app) |

## Repositories

| Repo | What it is |
|---|---|
| [agentic-project-factory](https://github.com/rb1whitney/agentic-project-factory) | Multi-agent swarm for infrastructure and cloud work. Skills, agent definitions, AST and graph tooling, and governance rules in one hub. |
| [nit-fabric](https://github.com/rb1whitney/nit-fabric) | Audits AWS and GCP connectivity: CIDR overlaps, VPC and BGP topology, security drift. Z3 solver for formal checks. |
| [cloud-boot-app](https://github.com/rb1whitney/cloud-boot-app) | Reference Java 21 / Spring Boot service on Kubernetes, managed with Terraform, Crossplane and Argo CD. |
| [vault_controller_example](https://github.com/rb1whitney/vault_controller_example) | Shell wrapper that keeps a HashiCorp Vault cluster in a declared state. |

## In progress

Rewriting agent skills as a typed contract plus a concrete action template, then measuring tokens and LLM calls against the prose originals. Results and method will be published here with the code.

## Writing

- Oct 2026: [One Platform Failed Our App Teams. The Other Failed Us.](https://medium.com/@rb1whitney/one-platform-failed-our-app-teams-the-other-failed-us-97cfcbd92f0b)
- Sep 2026: [Taming Multi-Agent Workflows](https://medium.com/@rb1whitney/taming-multi-agent-workflows-7eec951375cf)
- Sep 2026: [Stop Dumping Raw Code into LLMs: Why ASTs lead to Scalable AI Agents](https://medium.com/@rb1whitney/stop-dumping-raw-code-into-llms-why-semantic-graphs-lead-to-scalable-ai-agents-707c9c3220b0)
