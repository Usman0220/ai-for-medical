# AI for Medical

Learning AI for medicine — LLM-first, with a second project in classic ML. Built by a final-year MBBS student who can already code.

## Direction

Not MBBS exam prep. This repo is for learning how AI works in medicine and building with it — especially large language models — and using it safely as a doctor.

## The plan — LLM-first spine

An 8-week roadmap, ~1–2 hours a day, revision first (the PGET + FCPS Part I plan always comes before this):

| Phase | What | When |
|---|---|---|
| [Phase 0 — Setup](steps/phase-0-setup.md) | Python refresh, Colab GPU, this repo | Days 1–3 |
| [Phase 1 — How LLMs work](steps/phase-1-ml-foundations.md) | Tokens, transformers & attention (intuition), prompting, why they hallucinate | Weeks 1–2 |
| [Phase 2 — Building with LLMs](steps/phase-2-deep-learning.md) | API calls, structured output, embeddings + RAG over your own prep notes | Weeks 3–4 |
| [Phase 3 — Evaluation & safety](steps/phase-3-project.md) | Eval sets, scoring answers, calibration, bias/fairness, privacy, AI as a medical device | Weeks 5–6 |
| [Phase 4 — The small project](steps/phase-4-beyond.md) | LLM study assistant: RAG chatbot over revision notes, with citations and an "I don't know" | Weeks 7–8 |

## Second project — ECG rhythm classifier

After the LLM spine: classic ML → deep learning on PTB-XL, ending with a 1D-CNN that reads a 10-second ECG and classifies the rhythm. Steps in [steps/project-2-ecg-classifier.md](steps/project-2-ecg-classifier.md). The ML foundations live there as background, not the spine.

## Things to do

The full checklist lives in [TODO.md](TODO.md) — one checkbox per step, in order. Tick a box when a step is done.

## Weekly rhythm

- **Mon–Fri:** 45–60 min theory + 30 min code exercise.
- **Saturday:** project work only — no new theory.
- **Sunday:** 30-min checkpoint — what did I learn, what broke, what's next. Write 5 lines here.

If a week slips, don't restart — just continue from where you stopped. Consistency beats intensity.
