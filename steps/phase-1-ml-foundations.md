# Phase 1 — ML Foundations (Weeks 1–3)

## Week 1 — How learning works

- [ ] Supervised vs unsupervised vs reinforcement — with medical examples (diagnosis = supervised, patient clustering = unsupervised)
- [ ] Train / validation / test split — and why you must split by PATIENT, never by row (same patient in train + test = leakage)
- [ ] Overfitting — the "memorised past papers but can't answer a new question" problem
- [ ] Evaluation you already know: confusion matrix, sensitivity, specificity, PPV, NPV, ROC curve, AUC
- [ ] Exercise: predict diabetes from the Pima dataset — report sensitivity + specificity, not just accuracy

## Week 2 — The classic algorithms

- [ ] Linear regression → logistic regression (yes/no diagnosis as a probability)
- [ ] Decision trees → random forest → gradient boosting (the workhorses of tabular medical data)
- [ ] k-NN and SVM — when they help, when they don't
- [ ] Cross-validation + hyperparameter tuning (GridSearchCV)
- [ ] Exercise: heart-disease prediction (UCI) — compare logistic regression vs random forest vs XGBoost, same test set

## Week 3 — Unsupervised + the maths that matters

- [ ] Clustering (k-means) + dimensionality reduction (PCA) — e.g. grouping patients by lab patterns
- [ ] Maths, just-in-time: vectors & matrices (what a dataset IS), gradients (how models learn), Bayes' rule (why a positive test isn't always disease)
- [ ] Class imbalance: why 95% accuracy can be a lie when only 5% of patients have the disease — precision, recall, F1, PR curves
- [ ] Exercise: cluster patients, then explain the clusters in plain clinical words

## Main resources

- **Andrew Ng — Machine Learning Specialization** (Coursera) — the standard starting course, gentle maths. https://www.coursera.org/specializations/machine-learning-introduction
- **StatQuest** (YouTube) — best intuition-first explanations of every algorithm. https://www.youtube.com/@statquest
- **Book:** Aurélien Géron, *Hands-On Machine Learning with Scikit-Learn, Keras & TensorFlow* — the practical bible, keep it beside you all 8 weeks.
- **Book (short):** Andriy Burkov, *The Hundred-Page Machine Learning Book* — the whole field in one sitting.
