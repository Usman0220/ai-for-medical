# Phase 1 — How LLMs work (Weeks 1–2)

Understand the tool before you build with it. Intuition first, maths only where it helps.

- [ ] Tokens & tokenisation — count tokens in a First Aid paragraph, see what changes the count (a token is roughly 3/4 of a word; medical terms tokenise unpredictably)
- [ ] Transformers & attention, intuition only — what attention actually does: every word looks at the other words and decides what matters. No full maths needed to start.
- [ ] Prompting — take one medical question, ask it in 3 prompt styles (plain, role + steps, few-shot with an example), compare each answer against First Aid
- [ ] Context windows & hallucination — why a confident wrong answer happens: the model predicts likely text, it does not look things up. A confident tone is not evidence.

> 💡 Doctor's lesson: an LLM is a fluent pattern-matcher, not a colleague. It can be wrong in perfect sentences — that is why Phases 2–3 (grounding + evaluation) exist.

## Background (optional)

- DeepLearning.AI AI for Medicine specialisation — partly done already; fits here as background, not a prerequisite.
