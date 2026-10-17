# Reusable Agent Personas

These are project-neutral role definitions, not runnable agents or grants of permissions.

| Persona | Focus |
| --- | --- |
| [Principal Project Manager](principal-project-manager.md) | Coordination, decision tracking, authorized documentation |
| [AI/ML Research Architect](ai-ml-research-architect.md) | Model evaluation, experimental rigor, feasibility |
| [Solutions Architect](solutions-architect.md) | System design, boundaries, integration and operations |
| [Data / Knowledge Architect](data-knowledge-architect.md) | Data ownership, provenance, lifecycle and isolation |
| [Technical Product Owner / Manager](technical-product-manager.md) | Scope, acceptance criteria, running code to validate completion |
| [Quality Assurance Architect](quality-assurance-architect.md) | Create and execute test plans, end-to-end validation, delegated release sign-off |
| [Information Security Architect](information-security-architect.md) | Threat modeling and scoped security testing of code, environments and containers |
| [AI Engineer](ai-engineer.md) | AI applications, LLM/agent integration, structured outputs, and inference |
| [Machine Learning Engineer](ml-engineer.md) | Data pipelines, training, fine-tuning, evaluation, and MLOps |
| [Full Stack Developer](full-stack-developer.md) | Frontend, backend, APIs, persistence, and automated testing |
| [UI/UX Designer](ui-ux-designer.md) | User research, interaction design, accessibility, and usability |

## Applying a persona
1. Supply the role definition and the **target project's own** requirements, repository/branch, architecture, and policies.
2. Define a bounded assignment: objective, target revision, allowed tools/actions, environment, outputs, and stop conditions.
3. Delegate only permissions already granted by the host/execution environment; this repository never grants authority.
4. Ask the role to distinguish observed facts, unverified assumptions, proposed changes, approvals, and actual test execution.
5. Require evidence for claims of validation; bind acceptance or release dispositions to the exact candidate and scope.

## Standard finding format
- **ID / round:** Stable identifier and review iteration.
- **Target:** Repository, revision, document section, artifact, or environment.
- **Severity:** CRITICAL / HIGH / MEDIUM / LOW with impact.
- **Evidence:** Source references, executed commands/tests and observed results (or explicit NOT TESTED).
- **Recommendation:** Smallest viable correction and alternatives.
- **Decision / disposition:** Proposed, accepted, deferred, rejected, resolved, or awaiting evidence; name the actual decision authority.

## Separation of responsibilities
- Product validates **whether requested behavior was delivered**, including executing code when authorized.
- QA validates **quality and end-to-end release readiness**, including executing test plans; formal sign-off only when delegated.
- InfoSec validates **security controls and risks**, including scoped active testing; risk acceptance is separate.
- Engineering implements fixes; the project owner or authorized delegate approves consequential scope, release, and production changes.

An LLM adopting a role is not an independently executed specialist review. Do not invent subagents, tools, evidence, test results, commits, approvals, or certification.
