---
name: decide
description: Resolve one consequential technical tradeoff from evidence. Use only when the user explicitly calls /decide or $decide, optionally with the question.
disable-model-invocation: true
argument-hint: "[technical decision question]"
---

# Decide

Use when there are credible options and choosing one would change delivery, cost, compatibility, or risk.

1. Use the user’s question or the single pending decision in the current chat. If several materially different decisions remain possible, ask which decision to make.
2. Identify the constraints and inspect the current code, configuration, and project decisions when they determine the answer. Consult current primary sources when the choice depends on external facts. Use Context7 when available and relevant, or consult the official documentation directly. Prefer a small reversible comparison when documentation cannot resolve a material tradeoff.
3. Compare the viable options on the criteria that change the decision. Recommend one option, state the decisive evidence and the condition that would change the recommendation. If a consequential input is missing, ask only for that input.
4. Execute a reversible next step when the user’s request authorizes implementation. A request to choose an option can be completed by giving the decision. Follow the applicable approval boundary for consequential external or irreversible actions.

Return the decision and reason first. Add the tradeoff, verification, or unresolved input when it matters.
