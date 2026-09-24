# Delivery resources

<!-- AI TOUR TEMPLATE PLACEHOLDER: replace the required deck link before publication. Optional recording links can remain unavailable. -->

## How to deliver this session

🥇 Thanks for delivering this session!

Presenter and train-the-trainer materials for **BRK231 — Trusted AI at scale: Foundry to
Agent 365**. The session follows **Caldova Pharmaceuticals**, a fictional global
pharmaceutical company responding to a sudden manufacturing capacity gap. Caldova builds a
supplier intelligence agent in Microsoft Copilot Studio, optimizes an invoice assurance agent
in Microsoft Foundry, and governs its growing agent estate with Microsoft Agent 365.

Before you deliver the session, please:

1. Read this document and every linked resource in full.
2. Watch the full session recording and the per-demo clips, when available.
3. Open the delivery deck and review the Caldova storyline and the five acts.
4. Prepare the three demo environments (see [Prepare your environment](#-prepare-your-environment)).
5. Rehearse each demo end to end with the prompts in [`demos/`](demos/README.md).

## 📁 File summary

| Resource | Link | Description |
|---|---|---|
| Session delivery deck | [BRK231-AITourFY27.pdf](../BRK231-AITourFY27.pdf) | The session slides. Temporary repo link; replace with the public short link when available |
| Full session recording | Not yet available | The full session presentation |
| Demo flows | [demos/README.md](demos/README.md) | Per-demo walkthroughs and prompts |
| Scenario and reference | [../docs/README.md](../docs/README.md) | Caldova personas and the build, ground, secure and govern, and scale model |
| Attendee instructions | [../instructions/README.md](../instructions/README.md) | Self-paced path for attendees after the session |

## 🖥️ Demo videos

Select the demo instructions to see how to deliver each demo.

| # | Demo | Instructions | Clip — no audio | Clip — voice-over |
|---|---|---|---|---|
| 1 | Building a conversational agent using Microsoft Copilot Studio | [Demo instructions](demos/copilot-studio.md) | Not yet available | Not yet available |
| 2 | Optimizing the invoice assurance agent in Microsoft Foundry | [Demo instructions](demos/foundry.md) | Not yet available | Not yet available |
| 3 | Observe, onboard, and govern agents in Agent 365 | [Demo instructions](demos/agent-365.md) | Not yet available | Not yet available |

## Run of show

The deck is organized in five acts.

| Act | Slides | Content | Demo |
|---|---|---|---|
| 1 — Understand the AI scale challenge | 4–10 | Audience question, Caldova introduction and org chart, why pilots stall, one connected system to build, ground, secure and govern, and scale | — |
| 2 — Build conversational agents grounded in business data | 11–22 | Charlotte's supplier question, why customers build with Copilot Studio, connectors, hybrid automation, the GitHub Copilot harness, channels, the Copilot Studio model | [Demo 1](demos/copilot-studio.md) (slides 20–22) |
| 3 — Fine-tune AI models with business data and build AI apps and agents | 23–32 | Sarah's invoice assurance agent, the Microsoft Foundry optimization ladder, fine-tuning, traces to training data, small tuned model vs. frontier | [Demo 2](demos/foundry.md) (slides 31–32) |
| 4 — Govern your AI workloads | 33–58 | Carlos's enterprise-wide question, the agent registry, Agent 365 Observe, Govern, and Secure | [Demo 3](demos/agent-365.md) (slides 56–57) |
| 5 — What have we learned today? | 59–63 | Key takeaways, get started with Agent 365, next steps, repo QR code | — |

## 🏋️ Prepare your environment

### What these demos run on

- **Demo 1** — [Microsoft Copilot Studio](https://copilotstudio.microsoft.com), with a
  supplier intelligence agent grounded in Caldova's supplier contracts, sourcing policies, and
  supplier data.
- **Demo 2** — a [Microsoft Foundry](https://ai.azure.com) project with the
  `contract-policy-evidence` invoice assurance agent, its production traces, and fine-tuning.
- **Demo 3** — the [Microsoft 365 admin center](https://admin.microsoft.com) with Agent 365, and
  Microsoft Purview.

### Pre-flight checks

- Signed in to Copilot Studio, the Microsoft Foundry portal, the Microsoft 365 admin center, and
  Microsoft Purview with the demo accounts.
- The supplier intelligence agent answers Charlotte's supplier question in Copilot Studio.
- The `contract-policy-evidence` agent responds in the Foundry Playground and has traces.
- Tabs pre-opened for each demo.

## Support

Content owners: Dona Sarkar, Amy Boyd ([@amynic](https://github.com/amynic))
