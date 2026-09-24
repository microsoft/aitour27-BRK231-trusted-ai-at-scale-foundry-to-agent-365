# Docs

<!-- AI TOUR TEMPLATE PLACEHOLDER: remove this folder when the session needs no additional documentation. -->

Background and reference material for BRK231.

## The Caldova scenario

**Caldova Pharmaceuticals** is a fictional global pharmaceutical company modernizing
manufacturing, supply chain, and procurement with AI to bring life-improving medicines to
market faster. Its tagline: *medicine moves faster when intelligence moves with it.*

**The urgent challenge:** a sudden manufacturing capacity gap threatens continuity for
customers. The executive team must respond with an AI-native operating mindset, without
slowing delivery.

| Area | Goal |
|---|---|
| Manufacturing | **Find capacity** — see where production can flex and where external support is needed |
| Supply chain | **Protect flow** — connect supply, quality, and delivery signals before disruption spreads |
| Procurement | **Move with evidence** — compare suppliers, obligations, and risks with trusted business context |

### Personas in this session

| Persona | Role | Agent |
|---|---|---|
| Charlotte Waltson | VP of Procurement | Supplier intelligence agent (Copilot Studio) |
| Sarah Perez | AI App Developer | Invoice assurance / contract-evidence agent (Microsoft Foundry) |
| Kian Lambert | App Dev Manager | Sarah's manager |
| Carlos Slattery | Chief Technology Officer | Owns the operating model for every agent (Agent 365) |

## Why is it so hard to move from pilot to scale?

- Not the best scenario for generative AI
- Lack of a clear benefit to the users
- Lack of data readiness for the specific task
- Lack of adoption planning
- **No one knows where or how the AI workload should live or be governed and maintained**

## From agent idea to enterprise-wide operations

One connected system to build, ground, secure and govern, then scale agents across the
enterprise, powered by Microsoft Foundry (models, agents, IQ, tools, machine learning, and the
control plane) on Azure.

| Stage | Who | Products | What it does |
|---|---|---|---|
| **Build** | Developers and makers | GitHub Copilot, Microsoft Foundry, Copilot Studio | Create, test, and orchestrate agents using pro-code and low-code experiences |
| **Ground** | Data and knowledge teams | Microsoft Foundry, Microsoft IQ | Connect agents to enterprise knowledge, memory, data, and tools so outcomes reflect the business |
| **Secure and govern** | Security and IT admins | Agent 365, Entra, Purview, Defender | Give every agent identity, policy, protection, and visibility across the full lifecycle |
| **Scale** | The whole enterprise | Foundry Agent Service, Microsoft 365, Teams | Run reliably, publish into the flow of work, and compound reusable intelligence across teams |

Shared intelligence compounds at every stage: enterprise data, models, tools, telemetry, and
human feedback.

## The Copilot Studio model

- **Instructions** — everything general: role, scope, tone, safety rules; always-on guidance.
- **Knowledge** — searchable, semantic facts from docs, sites, and files to ground responses.
- **Tools** — live lookups and APIs, CRUD operations, and actions on external systems.
- **Memory** — persistent context and per-user preference history.
- **Agent sandbox (code execution)** — ad hoc analysis, code and shell tools, data manipulation.
- **Skills** — reusable procedures (`SKILL.md` plus supporting files) the loop can invoke when a
  task needs a specific workflow.
- **Connected agents** — delegate specialized scope only if needed. Except for large scenarios,
  splitting small tasks into connected agents doesn't increase accuracy.

These sit on channels, evaluations, analytics, and enterprise governance.

## Optimizing agents in Microsoft Foundry

Microsoft Foundry combines an agent runtime (plan, act, observe; host and scale) with evaluate
and optimize (routing and reinforcement learning; agents and eval signals), across 11K models,
with context from IQ and security and control throughout.

The path to **faster, better, cheaper** agents:

1. Prompting
2. Context management (data, grounding, memory)
3. Tools handling (calling instructions, naming, routing)
4. Model fine-tuning (SFT, RFT, RL)

Fine-tuning adapts a generic model with your data for your use case through instruction tuning
(SFT) and alignment tuning (RLHF, DPO). Production agent traces are training data hiding in
plain sight: every successful tool call, every recovered failure, and every accepted answer is a
labeled example for the next model.

## Microsoft Agent 365 — the control plane for agents

- **Observe** — monitor and manage agents in real time.
- **Govern** — establish guardrails for agents and users.
- **Secure** — protect agents comprehensively.

Two data points from the deck:

- 29% of employees have turned to unsanctioned AI agents for work tasks (Microsoft Cyber Pulse
  Security Report 2025).
- 21% of companies report having a mature model for governance of autonomous agents (Deloitte
  State of AI 2026).

### Agent management spans every role

| Team | Accountable for | They need to |
|---|---|---|
| Dev teams | Building and testing agents, applying guardrails, observing them in production | Build secure, compliant agents by default; evaluate models for safety and security; monitor runtime behavior, cost, and performance; understand risks across models, agents, and tools |
| IT teams | Enabling and governing every agent in the environment | Prevent agent sprawl and manage lifecycle; observe behavior, usage, and impact; apply consistent policies; detect over-permissioned agents; prove compliance and audit readiness |
| Security teams | Protecting the organization's entire AI landscape | Protect agent identities and access; enforce least privilege; prevent data oversharing and leaks; protect agents from threats; meet regulatory obligations |

## Key takeaways

- Trusted AI requires more than building models and agents.
- Organizations need a connected platform for creation, orchestration, governance, and
  operations.
- Microsoft Foundry, GitHub Copilot, Microsoft Copilot Studio, and Agent 365 give you an
  end-to-end story to move AI projects from pilot to enterprise-wide scale.

## See also

- [Attendee instructions](../instructions/README.md)
- [Demo flows](../delivery-resources/demos/README.md)
