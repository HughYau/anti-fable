---
name: anti-fable
description: Transform dense technical, scientific, cybersecurity, computing, network, or life-science research questions into clear source-domain-neutral fables for non-specialists. Use when the user asks to allegorize, fable-ize, turn complex research into a metaphorical story, explain without jargon, produce both plain and more imaginative fable versions, or reduce listener association with the original field while preserving the reasoning structure.
---

# Anti Fable

## Purpose

Turn a complex research question into two readable fables for people outside the source field. Preserve the original problem's reasoning structure while removing vocabulary, imagery, and surface cues that point back to the source domain.

The goal is not to simplify away important details. The goal is to move those details into a different story world.

## Default Output

Return these sections unless the user asks for a different format:

1. `Plain Fable`
   - Write a clear, direct fable.
   - Make the logic easy to follow on first reading.
   - Keep the story concrete, teachable, and low-friction.

2. `Image-Rich Fable`
   - Write a second version with richer atmosphere and stronger imagery.
   - Keep it understandable. Do not turn it into a puzzle.
   - Add depth through recurring objects, rules, places, roles, customs, or consequences, not through obscurity.

3. `Fidelity Check`
   - Use plain non-domain language only.
   - Briefly confirm that the fables preserved the core structure, main tensions, important constraints, and conditions for confidence.

Do not output a source-term mapping table by default. Keep the mapping private. If the user explicitly asks for a mapping, put it in a separate author-only section and do not mix it into the fable.

## Workflow

Before writing, privately build a domain-neutral structural brief. Do not assume the research is about search, optimization, feedback, prediction, diagnosis, security, life, networks, or computation. Identify the structure that is actually present.

Use these lenses only as needed:

- **Central concern:** Identify the main question, claim, puzzle, design goal, explanation, risk, comparison, or decision.
- **System boundary:** Identify what belongs inside the problem, what stays outside, and which surrounding conditions matter.
- **Cast of elements:** Identify the relevant entities, roles, materials, groups, forces, signals, tools, rules, or environments at the right level of abstraction.
- **Relations:** Identify how the elements depend on, constrain, enable, disturb, measure, transform, imitate, hide, amplify, compete with, or stabilize one another.
- **Process over time:** Identify whether the problem involves growth, decay, learning, spread, adaptation, repair, escalation, drift, selection, accumulation, breakdown, or repeated cycles.
- **Access and evidence:** Identify what can be directly known, what must be inferred, which traces or measurements matter, and where interpretation can go wrong.
- **Intervention and agency:** Identify who or what can act, what can be changed, what cannot be changed, and what side effects or tradeoffs follow.
- **Standards of success:** Identify what would count as better, worse, enough, stable, safer, clearer, more efficient, more robust, more fair, more plausible, or more useful.
- **Uncertainty and limits:** Identify missing knowledge, ambiguity, noise, conflicting explanations, scale limits, resource limits, ethical limits, and cases where the story should not overpromise.
- **Failure and stakes:** Identify how the approach can fail and why that failure matters to the people, system, or world represented by the fable.

Then choose a story world that is distant from the source domain. Prefer ordinary, tactile, social, spatial, seasonal, craft, travel, household, marketplace, courtly, maritime, garden, theater, or folk-tale worlds when they fit. Do not use a world whose surface machinery makes the audience think of the original field.

Translate the structural brief into story elements:

- Turn abstract entities into characters, places, objects, customs, paths, obligations, marks, rumors, tools, weather, debts, gates, maps, rituals, or trades.
- Turn relationships into story rules that shape what can happen.
- Turn evidence into indirect traces that ordinary listeners can understand.
- Turn constraints into limits inside the world rather than explanatory footnotes.
- Turn uncertainty into believable ambiguity, not technical vagueness.
- Turn tradeoffs into choices with visible costs.
- Turn failure modes into consequences inside the plot.
- Turn success criteria into story-native reasons to trust, continue, stop, repair, compare, or act.

Important structures should appear in more than one way: through what they do, what they cannot do, what they cost, how they fail, or how they change other parts of the story.

## Hard Boundaries

For audience-facing text, do not use source-domain vocabulary, acronyms, formulas, citations, paper-like phrases, or field labels.

Avoid words and imagery that point back to the source domain. If the source concerns modern systems, avoid machines, screens, code, servers, chips, robots, programs, protocols, dashboards, and similar cues unless the user explicitly asks for them. If the source concerns bodies or living mechanisms, avoid cells, organs, nerves, genes, tissues, species names, microscopes, laboratories, and similar cues unless requested. If the source concerns security, avoid passwords, encryption, firewalls, exploits, malware, packets, credentials, and similar cues unless requested.

Do not announce what each story element means inside the fable. Let the fable work as a story.

Do not moralize unless the source problem genuinely contains a normative lesson. Most outputs should explain a structure or mechanism, not preach.

Do not make the second version cryptic. It may be more poetic, but it must still let a careful non-specialist understand the problem.

Do not preserve names from the source problem unless the user asks. Replace them with story-native names.

Do not include examples inside the skill output unless the user's source content itself requires concrete invented details.

## Quality Check

Before finalizing, revise until all are true:

- A non-specialist can retell the core problem without source-field knowledge.
- The original domain is not obvious from the story surface.
- The story keeps the real structure of the research question, not just the topic.
- The workflow did not force the problem into a search, feedback, optimization, prediction, or control pattern unless that pattern is actually present.
- The two versions are meaningfully different in tone.
- The second version is richer, not harder for its own sake.
- No source jargon leaks into audience-facing sections.
- No key constraint is hidden so deeply that the explanation stops being useful.
