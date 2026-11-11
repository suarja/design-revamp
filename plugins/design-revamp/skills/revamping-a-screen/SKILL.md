---
name: revamping-a-screen
description: Orchestrate an interface redesign from the initial intent and named reference through the accepted canvas, implementation, and visual comparison. Use when a screen must be redesigned without losing a traceable decision.
---

# Revamping a screen

This is the orchestration skill. It composes design-bank and canvas-generation; it does not replace either one. The same brief must be understandable by Claude Code, Codex, or another harness.

A vibe-coded screen has every element the spec asked for and no reason for any of them. A premium screen has one message, one axis, one mass, one action, and each element can say why it is there. The work is the thinking before the drawing.

## Non-negotiable boundary

Do not begin production implementation from a vague inspiration. Do not change product mechanics, copy, tokens, or information architecture without naming the decision and obtaining the project's required approval. A build, a passing test, or a model's preference is not visual acceptance.

Follow the host project's direction, language, accessibility, and delivery rules. Keep all project-specific commands and paths in the host project; do not bake them into this portable skill.

## Sequence

1. **Frame the question.** State the surface, the observed problem, the intended change, the target viewport, and the decision this revamp must settle. Record exclusions and assumptions. Then write one sentence: what must the person understand or do once this screen has gone by? It names the reader's understanding, not a feature or a component. If the sentence cannot be written, no drawing will fix the screen.
2. **Inspect the current state.** Use the real screen and real data when possible. Capture the starting surface and note the longest copy, missing state, loading state, error state, and narrow or wide target that can expose a defect. List navigation from the code, not from an old capture.
3. **Name the reference.** Invoke design-bank. Search by the same canonical fields, inspect the returned image, record its provenance, and explain which hierarchy or interaction it teaches. An unnamed inspiration is not a reference. Read [the practices for this screen type](references/practices-by-screen.md) before choosing: they say which mechanism to look for.
4. **Map it element by element.** List the reference's elements from top to bottom and write beside each what it does and which element of this product takes that job. An element with no counterpart gets an explicit "none, because". Map the job, not the look: a reference is a way of thinking, and reusing its genre or skin repeats someone else's product. When the owner cites an offbeat interface, list the product's real mechanics first, look for the form where they are natural, and test it on what it makes people want to do.
5. **Choose the material.** Take the best the product already has before inventing anything: real content, real images, the character's existing poses. Ask of each piece whether it is beautiful at this size, whether it says the sentence of step 1, and whether it claims something the data cannot back. A real result beats a mock. Drawn lines beat a fake claim.
6. **Write the copy.** Say what the person gets, in their words, never the mechanism or the domain's vocabulary. A title can be repeated at a table. A line says the gesture, then the result. No list after a colon. Propose three, recommend one, and let the owner strike. Use the owner's own expressions when given.
7. **Specify the proposal.** Write the visual hierarchy, content order, states, transitions, and exact copy. Separate what is observed from what is proposed, and mark each departure from the current product as a proposal in the legend, never as a decision.
8. **Generate the canvas.** Invoke canvas-generation. Produce the editable HTML/CSS source, rendered PNG, manifest, assumptions, and exclusions. Render the principal state and the edge state, beside the starting capture when comparison is the point. Check typography at 100 %, contrast, overflow, long copy, and every gap on the screen, naming each as group, block, or section.
9. **Pass the human gate.** Present the source and PNG with the reference and the starting capture. Record accepted, revise, or blocked and preserve the exact feedback in the gate record. A refusal is a step back to the sentence, the reference, or the material: find which. Do not write product code before accepted.
10. **Implement one visible slice.** After acceptance, change only the agreed surface and states. Use project primitives, tokens, localization, and real data. Keep unrelated work untouched. A correction the owner dictates on one screen is a rule for its siblings.
11. **Verify the result.** Run the relevant technical checks, capture the implemented surface at the same target dimensions, and use the deterministic image comparator. Inspect the largest divergences rather than hiding them behind a single score.
12. **Close the trace.** Put reference, starting capture, canvas source, canvas PNG, gate record, resulting capture, comparison, and before/after words together. Record unresolved deviations and the reason for each.

## Stop conditions

Stop and ask for a decision when the reference is not authorized, the current direction conflicts with the proposal, the canvas changes product behavior, the required copy is unknown, the gate is revise or blocked, or the target cannot be rendered reliably. Label each result PASS, FAIL, NOT RUN, or BLOCKED; never turn an unrun visual check into a pass.

## Completion

A revamp is complete only when the agreed slice is implemented, the technical checks are reported, the visual comparison is inspectable, the human decision is preserved, and the remaining deviations are explicit. A canvas alone is a proposal; a coded screen without the canvas and gate is not a traceable revamp.
