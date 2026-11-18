# Project 2 — ECG rhythm classifier (after the LLM spine)

The classic-ML second project. Do this after the LLM spine, not before it.

## What

A model that reads a 10-second ECG and classifies the rhythm — Normal, Atrial Fibrillation, Myocardial Infarction, etc.

**Why this one:** you already read ECGs clinically, the data is free and clean, 1D signals train fast on Colab, and it's a genuinely impressive portfolio piece.

**Data:** PTB-XL — 21,837 12-lead ECGs, free on PhysioNet. https://physionet.org/content/ptb-xl/1.0.3 (MIT-BIH arrhythmia database is the classic alternative.)

## Background A — ML foundations

- [ ] Supervised vs unsupervised vs reinforcement — with medical examples (diagnosis = supervised, patient clustering = unsupervised)
- [ ] Train / validation / test split — and why you must split by PATIENT, never by row (same patient in train + test = leakage)
- [ ] Overfitting — the "memorised past papers but can't answer a new question" problem
- [ ] Evaluation you already know: confusion matrix, sensitivity, specificity, PPV, NPV, ROC curve, AUC
- [ ] Linear regression → logistic regression (yes/no diagnosis as a probability)
- [ ] Decision trees → random forest → gradient boosting (the workhorses of tabular medical data)
- [ ] k-NN and SVM — when they help, when they don't
- [ ] Cross-validation + hyperparameter tuning (GridSearchCV)
- [ ] Clustering (k-means) + dimensionality reduction (PCA) — e.g. grouping patients by lab patterns
- [ ] Maths, just-in-time: vectors & matrices (what a dataset IS), gradients (how models learn), Bayes' rule (why a positive test isn't always disease)
- [ ] Class imbalance: why 95% accuracy can be a lie when only 5% of patients have the disease — precision, recall, F1, PR curves
- [ ] Exercise: predict diabetes from the Pima dataset — report sensitivity + specificity, not just accuracy; then heart-disease prediction (UCI) — compare logistic regression vs random forest vs XGBoost, same test set

## Background B — Deep learning & medical data

- [ ] Perceptron → MLP → backpropagation — watch 3Blue1Brown's neural network series first (visual, no equations needed to start)
- [ ] PyTorch basics: tensors, autograd, training loop — build a tiny network that classifies tabular data
- [ ] Activation functions, loss functions, optimizers (Adam), learning rate — what each knob actually does
- [ ] CNNs: convolution, pooling — why they work on X-rays and why they work on ECG traces too (1D convolution)
- [ ] Data augmentation for medical images + transfer learning (start from a pre-trained model, fine-tune on medical data)
- [ ] Know your datasets: PTB-XL (ECG), MIT-BIH (arrhythmia), NIH ChestX-ray14, CheXpert, MIMIC (needs credentialing — later)
- [ ] Exercise: train a CNN to spot pneumonia on a small chest X-ray set — then look at what it gets WRONG, like a clinician reviewing a colleague

## Milestones

- [ ] Download PTB-XL, load it, plot 5 ECGs from each class — look at the data like a doctor before any model touches it
- [ ] Baseline model — logistic regression / random forest on simple features (heart rate, QRS width). Split by patient. Record sensitivity + specificity per class
- [ ] 1D-CNN in PyTorch on the raw signal — beat the baseline, check the confusion matrix: which rhythms get confused, and does that match clinical reality?
- [ ] Write-up + demo — a short README (problem, data, method, results, limits) and a tiny Gradio/Streamlit demo where you upload an ECG and it predicts. Push it to GitHub

## Resources

- **Andrew Ng — Machine Learning Specialization** (Coursera) — the standard starting course, gentle maths. https://www.coursera.org/specializations/machine-learning-introduction
- **StatQuest** (YouTube) — best intuition-first explanations of every algorithm. https://www.youtube.com/@statquest
- **Book:** Aurélien Géron, *Hands-On Machine Learning with Scikit-Learn, Keras & TensorFlow* — the practical bible.
- **Book (short):** Andriy Burkov, *The Hundred-Page Machine Learning Book* — the whole field in one sitting.
- **3Blue1Brown — Neural Networks** (YouTube playlist) https://www.youtube.com/playlist?list=PLZHQObOWTQDNU6R1_67000Dx_ZCJB-3pi
- **fast.ai — Practical Deep Learning** (free) https://www.fast.ai — build first, theory second
- **PyTorch tutorials** https://pytorch.org/tutorials
- **PhysioNet** (medical datasets) https://physionet.org
