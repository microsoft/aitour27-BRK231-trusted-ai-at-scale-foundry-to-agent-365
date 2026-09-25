# Demo 2 — Optimizing the invoice assurance agent in Microsoft Foundry

> Recording: not yet available · Deck: slides 24–32

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

- The [Microsoft Foundry portal](https://ai.azure.com) → the `contract-policy-evidence` agent
  (Playground, Traces, Evaluation, and Optimize tabs)

## Before you start

- The `contract-policy-evidence` agent is deployed (the recording uses `gpt-5.4-mini`) and has
  production traces.

## Steps

_Add the click-by-click steps after recording._

## Questions used

> Can we maintain the quality of our agent but scale it further without increasing cost and
> latency?

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

## Transcript

_After recording, paste the final timed transcript here._
