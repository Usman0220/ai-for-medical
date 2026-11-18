# Phase 3 — The Small Project (Weeks 5–8)

## Recommended project: ECG Rhythm Classifier

**What:** a model that reads a 10-second ECG and classifies the rhythm — Normal, Atrial Fibrillation, Myocardial Infarction, etc.

**Why this one:** you already read ECGs clinically, the data is free and clean, 1D signals train fast on Colab, and it's a genuinely impressive portfolio piece.

**Data:** PTB-XL — 21,837 12-lead ECGs, free on PhysioNet. https://physionet.org/content/ptb-xl/1.0.3 (MIT-BIH arrhythmia database is the classic alternative.)

## Milestones

- [ ] **Week 5:** download PTB-XL, load it, plot 5 ECGs from each class — look at the data like a doctor before any model touches it
- [ ] **Week 6:** baseline model — logistic regression / random forest on simple features (heart rate, QRS width). Split by patient. Record sensitivity + specificity per class
- [ ] **Week 7:** 1D-CNN in PyTorch on the raw signal — beat the baseline, check the confusion matrix: which rhythms get confused, and does that match clinical reality?
- [ ] **Week 8:** write-up + demo — a short README (problem, data, method, results, limits) and a tiny Gradio/Streamlit demo where you upload an ECG and it predicts. Push it to GitHub

## If you'd rather build something else

- **Chest X-ray pneumonia detector** — NIH ChestX-ray14, classic CNN project, very visual demo.
- **Diabetes / heart-disease risk predictor** — tabular data, simplest first win, good if you want a finished project in 2 weeks.
- **RAG chatbot over your own notes** — your gynae/obs banks as the knowledge base; ask it exam questions. More LLM, less ML-from-scratch. (This is the closest option to the LLM-for-medical direction.)
