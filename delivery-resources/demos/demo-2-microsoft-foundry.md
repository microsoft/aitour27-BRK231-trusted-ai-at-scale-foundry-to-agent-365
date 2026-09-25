# Demo 2 — Optimizing the invoice assurance agent (Microsoft Foundry portal)

> Recording: [Demo - no audio](../assets/demo-2-microsoft-foundry-no-audio.mp4) · [Demo - with audio](../assets/demo-2-microsoft-foundry-with-audio.mp4) · Deck: slides 24–32 ([PPTX](../assets/BRK231-AITourFY27.pptx) · [PDF](../assets/BRK231-AITourFY27.pdf))

## Demo video

### Demo - with audio

<video src="../assets/demo-2-microsoft-foundry-with-audio.mp4" controls width="100%"></video>

Can't see the player? [Open Demo - with audio](../assets/demo-2-microsoft-foundry-with-audio.mp4).

### Demo - no audio

<video src="../assets/demo-2-microsoft-foundry-no-audio.mp4" controls width="100%"></video>

Can't see the player? [Open Demo - no audio](../assets/demo-2-microsoft-foundry-no-audio.mp4).

## What this demo shows

Invoices from contract manufacturers rarely match their governing agreements. Sarah Perez, AI
App Developer, built an invoice assurance agent that proves what each invoice line is supported
by. She tells her manager, Kian Lambert, that they've hit a quality ceiling, and every new model
adds cost per assurance request.

The **contract-evidence agent** is grounded in contracts, policies, and prior assurance findings.

1. **Retrieve** — pulls relevant clauses, pricing schedules, rate cards, and policies using
   Foundry IQ.
2. **Evidence** — links each invoice line to the governing contractual evidence.
3. **Optimize** — fine-tunes a smaller model on production agent traces in Microsoft Foundry.

The optimization path: **production traces → filter and curate → training dataset →
fine-tuned model**.

## Where the demo happens

| The video shows… | In… |
|---|---|
| Chatting with the `contract-policy-evidence` agent | Microsoft Foundry portal — Playground |
| Production traces and evaluation results | Microsoft Foundry portal — Traces and Evaluation tabs |
| Fine-tuning a smaller model from the traces | Microsoft Foundry portal — Optimize tab |

## Before you start

- Play this demo from the video. Don't run it live.
- Narrate over **Demo - no audio**, or play **Demo - with audio**.
- The recording uses `gpt-5.4-mini` as the agent's model.

## Questions used

| Ask | Source |
|---|---|
| Can we maintain the quality of our agent but scale it further without increasing cost and latency? | Framing question for the demo |

Sample input shown in the Playground:

```text
S07-scn-sup-007-storage-after-close invalid_storage_period INV-SUP-007-2026-10
```

## Expected result

- **Assurance check** — invoice lines matched to supporting clauses and prior findings.
- **Evaluation outcome** — acceptable quality, but increasing cost and latency at scale.
- **Fine-tuning** — production agent traces distilled into a smaller, cheaper model.

**Outcome:** faster, defensible invoice assurance at lower cost.

> Slide 30 compares a tuned small model with frontier models. Its figures come from an internal
> benchmark by the MAI Frontier Tuning team; present them as stated on the slide.
