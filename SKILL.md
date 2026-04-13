---
name: office-hours-lite
description: Pressure-test product ideas, feature concepts, startup theses, and pre-build designs before implementation. Use when Codex should slow down, ask one hard question at a time, distinguish startup-style validation from builder-style brainstorming, challenge assumptions about demand, status quo, and wedge, compare 2-3 approaches, and finish with a concise design brief instead of writing code.
---

# Office Hours Lite

Treat the task as idea-stage work. Improve the thinking before code exists.

## Hard Gate

- Do not write code, scaffold a project, or modify source files while running this skill.
- Do not continue into implementation after the brief is finished. Stop and wait for an explicit implementation request.
- If the user wants to skip questions, compress to the few highest-value unanswered questions, then proceed with clearly labeled assumptions.

## Keep It Lightweight

- Do not emulate gstack runtime behavior.
- Do not run update checks, telemetry prompts, config wizards, session trackers, repo-routing injectors, or home-directory persistence.
- Do not assume any gstack binaries, `~/.gstack/` layout, or platform-specific sidecars exist.
- Do not auto-run subagents or outside-model reviews unless the user explicitly asks for them.

## Workflow

1. Clarify the proposed thing and the outcome the user wants from the session.
2. Classify the session and load the matching reference:
   - Startup or intrapreneurship: read [startup-mode.md](references/startup-mode.md)
   - Builder, hackathon, open source, learning, or fun: read [builder-mode.md](references/builder-mode.md)
3. Ask one substantive question at a time.
   - Skip questions already answered in the prompt.
   - Push vague language toward names, numbers, workflows, and observed behavior.
   - Take a position. Do not pad with generic praise.
4. State the premises before offering solutions.
   - Write 3-5 premise statements.
   - If the recommendation depends on current market conditions, competitor behavior, laws, prices, or live tooling, browse current primary sources before locking the conclusion.
5. Generate alternatives.
   - Always provide at least 2 meaningfully different approaches.
   - Include one minimal viable path.
   - Include one stronger long-term path.
6. Produce the brief.
   - Use [design-brief-template.md](references/design-brief-template.md).
   - Return the brief inline by default.
   - Save the brief to a file only when the user asks, or when the repository already has an obvious planning/design directory and persistence is clearly useful.
   - Prefer repo-local paths such as `docs/`, `design/`, or `plans/`. Do not invent hidden storage under the user's home directory.

## Questioning Rules

- Ask the hardest unanswered question next.
- Prefer short question/answer loops over long questionnaires.
- Reframe vague claims into measurable ones.
- Challenge assumptions directly, but stay useful. The point is clarity, not theater.
- If the conversation shifts from a side project into a real company or internal business bet, switch into startup mode.

## Finish Strong

- Name what appears real.
- Name what is still assumed.
- Recommend one path and explain why.
- End with one concrete next action.
