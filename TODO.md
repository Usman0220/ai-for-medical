# Things to do

The full checklist, in order. Tick a box when a step is done. Detail for each step lives in [`steps/`](steps/).

## Phase 0 — Setup (Days 1–3)

- [ ] Python refresh: numpy, pandas, matplotlib — one hour each, on real medical data
- [ ] Set up Google Colab — test a GPU notebook once
- [x] Create this GitHub repo (done 18 Nov 2026)
- [ ] Install once: `pip install scikit-learn pandas numpy matplotlib seaborn torch wfdb`

## Phase 1 — ML Foundations (Weeks 1–3)

- [ ] Week 1: supervised vs unsupervised vs reinforcement; train/validation/test split by patient; overfitting; confusion matrix, sensitivity, specificity, PPV, NPV, ROC, AUC; exercise — predict diabetes (Pima), report sensitivity + specificity
- [ ] Week 2: logistic regression; trees → random forest → gradient boosting; k-NN and SVM; cross-validation + GridSearchCV; exercise — heart-disease prediction (UCI), compare three models
- [ ] Week 3: k-means + PCA; just-in-time maths (vectors, gradients, Bayes); class imbalance (precision, recall, F1, PR curves); exercise — cluster patients, explain clusters clinically

## Phase 2 — Deep Learning & Medical Data (Weeks 4–5)

- [ ] Week 4: perceptron → MLP → backpropagation (3Blue1Brown first); PyTorch basics; activations, loss, optimizers, learning rate
- [ ] Week 5: CNNs (incl. 1D for ECG); augmentation + transfer learning; know PTB-XL, MIT-BIH, ChestX-ray14, CheXpert, MIMIC; exercise — pneumonia CNN, review its mistakes

## Phase 3 — The Small Project (Weeks 5–8)

- [ ] Week 5: download PTB-XL, load it, plot 5 ECGs per class
- [ ] Week 6: baseline model (logistic regression / random forest), split by patient, sensitivity + specificity per class
- [ ] Week 7: 1D-CNN in PyTorch, beat the baseline, check the confusion matrix
- [ ] Week 8: write-up + Gradio/Streamlit demo, push to GitHub

## Phase 4 — Beyond the Project (Ongoing)

- [ ] LLMs in medicine: transformers, RAG, medical chatbots, ambient scribes; hallucination as a patient-safety issue
- [ ] Read one paper a week (start: Microsoft MAI-DxO)
- [ ] Evaluation & safety: calibration, fairness, AI as a medical device
- [ ] Second project — e.g. the RAG chatbot over your own notes
