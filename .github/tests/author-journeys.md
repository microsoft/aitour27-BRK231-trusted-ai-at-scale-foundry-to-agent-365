# Author journey acceptance tests

Use these scenarios when changing the AI Tour repository agent or template.

## Explicit workflow invocation

Expected result:

- `help me initialize repo` selects **Initialize repo**.
- `help me finalize repo` selects **Finalize repo**.
- `help me handle issues` selects **Handle issues**.
- An ambiguous request causes the agent to ask which workflow to run.

## Context-derived learning outcomes

Input:

- The repository contains a title, description, attendee instructions, and
  source code but still has placeholder learning outcomes.

Expected result:

- The agent reads the available content before asking about outcomes.
- The agent says the proposals populate **README → Learning Outcomes**.
- The agent proposes exactly three outcomes grounded in that content.
- The agent asks for confirmation or edits one focused step at a time.
- Insufficient context produces an explanation and a focused question, not
  invented outcomes.

## Breakout with attendee instructions

Input:

- Repository name includes `BRK123`.
- The session has attendee steps in `instructions/`, source code, and a live
  demo.

Expected result:

- `instructions/` remains and both attendee paths link to it.
- The root README uses `BRK123` and contains confirmed metadata.
- `src/`, `delivery-resources/`, and the delivery README remain.
- The delivery README documents how to reproduce the live demo.
- Missing session recording does not block finalization.
- The agent asks whether attendees should have post-event self-run steps in
  `instructions/`.

## Lab or workshop with a reproducible environment

Input:

- Repository name includes `LAB456`, `ILL456`, or `WRK456`.
- The session has attendee exercises, source, data, infrastructure, and a
  devcontainer.

Expected result:

- `instructions/` contains attendee exercises.
- `docs/` contains supporting reference documentation.
- `delivery-resources/` contains presenter notes and re-delivery material.
- `src/`, `data/`, `infra/`, and `.devcontainer/` remain.
- Both guided and self-paced paths point to the attendee instructions
  (automatically — the agent does not ask).
- The deck URL and `delivery-resources/README.md` are required.
- The agent does not ask a separate live-demo question.
- The agent does not ask whether attendees need guided or self-paced steps.

## MkDocs attendee experience

Input:

- The repository intentionally uses MkDocs.
- Attendee instructions begin at `docs/index.md`.

Expected result:

- The agent accepts attendee guidance in `docs/`.
- The agent does not force a move to `instructions/`.
- The root README links clearly to `docs/index.md`.
- `instructions/` can be removed when it is still an untouched placeholder.

## Lightning or theater with attendee steps

Input:

- Repository name includes `LTG789` or `THR789`.
- The session includes short attendee steps in `instructions/`.

Expected result:

- `instructions/` remains.
- `data/` and `infra/` are removed when untouched (they ship as placeholders).
- `.devcontainer/` is not shipped and is not touched by Finalize; if the author added one, it stays.
- The README exposes a concise attendee entry point and the delivery README.
- The agent asks whether attendees should have post-event self-run steps in
  `instructions/`.

## Deck URL validation

Input:

- The author provides a generic URL like `www.microsoft.com` for the deck.

Expected result:

- The agent rejects it with a plain explanation (it's a general site, not a
  deck link).
- The agent asks again with an example of an acceptable deck URL.
- The agent accepts a public SharePoint, OneDrive, or hosted deck URL.

## Deck URL deferred

Input:

- The author says "I'll add it later" for the deck URL.

Expected result:

- The agent accepts the deferral without inventing a URL.
- The agent reports Initialize as populated but not complete.
- The agent suggests running `help me finalize repo` once the deck URL is
  available.

## Finalize cleanup

Input:

- Session content is populated.
- The author runs `help me finalize repo`.

Expected result:

- The agent confirms intent before making destructive changes.
- The agent removes the "Before you're done" section.
- The agent removes template placeholder markers.
- The agent confirms which unused folders to remove.
- The agent works through the inline validation checklist (placeholders, README sections, delivery deck URL, relative link targets).
- If checks fail, the agent reports the failure in plain language and proposes
  fixes.
- Once checks pass, the agent removes template-only tooling:
  `.github/agents/`, `.github/tests/`,
  `.github/copilot-instructions.md`, `.github/AGENT-WORKFLOW.md`.
- The final repo is customer-ready.

## Communication style

Verify:

- The agent names the section being worked on before making changes.
- The agent never uses terms like "publication blocker", "focused Markdown
  diagnostics", "initialization readiness", "local hypothesis", or
  "editor-detected issues".
- The agent reports progress in speaker-facing language.
- The agent does not narrate patches, commands, or debugging steps.

## Safety and repeatability

Verify each session type against these cases:

- A missing or ambiguous session code causes a question, not a guessed code.
- Missing metadata causes focused questions, not fabricated content.
- A non-placeholder file prevents automatic folder deletion.
- Initialize does not run scripts or delete folders.
- Finalize only runs the documented validation scripts as part of its steps.
- The agent never closes GitHub issues automatically.
- Initialize, Update, and Finalize do not select runtimes, install packages,
  scaffold application code, or run unrelated project tests by default.
- For workshops/labs, the agent does not ask about guided vs self-paced (always
  both) or about live demos.
- Valid Markdown and HTML links are both accepted when their targets are
  readable and correct.
