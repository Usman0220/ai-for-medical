# Phase 4 — The small project (Weeks 7–8)

## LLM study assistant

**What:** a RAG chatbot over your own revision notes — ask it exam questions, it answers from your notes, with citations.

**Why this one:** you already have the knowledge base (prep library, bits, banks, error log), it helps your revision directly, and "answers only from the notes, with citations" is the honest version of a medical chatbot.

**Rules for the assistant:**
- Answer only from the retrieved notes — cite the note for every claim.
- If the notes don't cover the question, say "I don't know" — never invent.
- Keep a log of every question it got wrong, so the eval set grows.

## Milestones

- [ ] LLM study assistant — RAG chatbot over revision notes, citations + "I don't know" behaviour
- [ ] Write-up + demo — a short README (problem, data, method, results, limits) and a tiny Gradio/Streamlit demo. Push it to GitHub

## After this

- A second project — e.g. the ECG classifier ([Project 2](project-2-ecg-classifier.md)), or a triage model — turns one project into a track record.
- Health-tech / AI roles value a portfolio over certificates — this project IS the portfolio. The UK Digital Health & AI Fellowship (~8 weeks, takes clinicians with zero tech background) is a real next step, and a first role can come in 6–12 months.
