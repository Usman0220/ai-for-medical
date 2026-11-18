# Phase 3 — Evaluation & safety (Weeks 5–6)

This is what separates a toy from a tool a doctor can trust.

- [ ] Build a 20-question eval set from revision topics, with correct answers (use your own error-log topics — the ones you got wrong are the best test)
- [ ] Score two approaches (plain prompt vs RAG) on the eval set — same questions, same marking. RAG should win on grounded questions; note where it doesn't.
- [ ] Calibration, bias/fairness, privacy — what can go wrong with patient data: overconfident wrong answers, worse performance on under-represented groups, never putting real patient data into a public model
- [ ] Read one paper: Microsoft MAI-DxO — critique it like a journal club: what was the test set, who were the comparators, what would break in a real ER?

> 💡 Doctor's lesson: hallucination is a patient-safety issue, not just an annoyance. A model that is confidently wrong on a rare case is dangerous in a way a wrong textbook never is. Evaluation, calibration and bias matter more than the headline number.
