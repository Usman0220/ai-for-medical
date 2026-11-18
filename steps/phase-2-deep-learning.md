# Phase 2 — Building with LLMs (Weeks 3–4)

Start building. Every step uses your own medical material.

- [ ] First API call — ask an LLM a medical question from Python, print the answer
- [ ] Structured output — force JSON answers (e.g. diagnosis + differentials + red flags) so the output is machine-readable, not prose to parse
- [ ] Embeddings + RAG — turn your own prep notes into searchable chunks, retrieve the relevant ones, and make the model answer with citations to the note it used
- [ ] Exercise — RAG over prep notes: 10 questions, check every cited answer against the note. A wrong citation is a fail, even if the answer looks right.

> 💡 The knowledge base is the point: your gynae/obs banks, your bits files, your error log — the model is only as good as what it can retrieve.
