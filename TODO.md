# Things to do

The full checklist, in order. Tick a box when a step is done. Detail for each step lives in [`steps/`](steps/).

## Phase 0 — Setup (Days 1–3)

- [ ] Python refresh: numpy, pandas, matplotlib — one hour each, on real medical data
- [ ] Set up Google Colab — test a GPU notebook once
- [x] Create this GitHub repo (done 18 Nov 2026)

## Phase 1 — How LLMs work (Weeks 1–2)

- [ ] Tokens & tokenisation — count tokens in a First Aid paragraph, see what changes the count
- [ ] Transformers & attention, intuition only — what attention actually does, no full maths
- [ ] Prompting — same medical question, 3 prompt styles, compare answers against First Aid
- [ ] Context windows & hallucination — why a confident wrong answer happens

## Phase 2 — Building with LLMs (Weeks 3–4)

- [ ] First API call — ask an LLM a medical question from Python, print the answer
- [ ] Structured output — force JSON answers (e.g. diagnosis + differentials + red flags)
- [ ] Embeddings + RAG — retrieve from his own prep notes, answer with citations
- [ ] Exercise — RAG over prep notes: 10 questions, check every cited answer

## Phase 3 — Evaluation & safety (Weeks 5–6)

- [ ] Build a 20-question eval set from revision topics, with correct answers
- [ ] Score two approaches (plain prompt vs RAG) on the eval set
- [ ] Calibration, bias/fairness, privacy — what can go wrong with patient data
- [ ] Read one paper: Microsoft MAI-DxO — what it actually showed

## Phase 4 — The small project (Weeks 7–8)

- [ ] LLM study assistant — RAG chatbot over revision notes, citations + "I don't know" behaviour
- [ ] Write-up + demo, push to GitHub

## Project 2 — ECG rhythm classifier (after the LLM spine)

- [ ] ML foundations (background): supervised vs unsupervised; train/validation/test split by patient; overfitting; confusion matrix, sensitivity, specificity, PPV, NPV, ROC, AUC; logistic regression, trees, random forest, gradient boosting; cross-validation + GridSearchCV; class imbalance
- [ ] Deep learning (background): perceptron → MLP → backpropagation; PyTorch basics; CNNs incl. 1D for ECG; transfer learning; know PTB-XL, MIT-BIH
- [ ] Download PTB-XL, load it, plot 5 ECGs per class
- [ ] Baseline model (logistic regression / random forest), split by patient, sensitivity + specificity per class
- [ ] 1D-CNN in PyTorch, beat the baseline, check the confusion matrix
- [ ] Write-up + Gradio/Streamlit demo, push to GitHub

## Later, optional

- DeepLearning.AI AI for Medicine specialisation — partly done already; placement still open, fits as background for Phases 2–3, not a prerequisite
