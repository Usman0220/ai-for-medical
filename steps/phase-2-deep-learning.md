# Phase 2 — Deep Learning & Medical Data (Weeks 4–5)

## Week 4 — Neural networks

- [ ] Perceptron → MLP → backpropagation — watch 3Blue1Brown's neural network series first (visual, no equations needed to start)
- [ ] PyTorch basics: tensors, autograd, training loop — build a tiny network that classifies tabular data
- [ ] Activation functions, loss functions, optimizers (Adam), learning rate — what each knob actually does

## Week 5 — Images & signals (the medical part)

- [ ] CNNs: convolution, pooling — why they work on X-rays and why they work on ECG traces too (1D convolution)
- [ ] Data augmentation for medical images + transfer learning (start from a pre-trained model, fine-tune on medical data)
- [ ] Know your datasets: PTB-XL (ECG), MIT-BIH (arrhythmia), NIH ChestX-ray14, CheXpert, MIMIC (needs credentialing — later)
- [ ] Exercise: train a CNN to spot pneumonia on a small chest X-ray set — then look at what it gets WRONG, like a clinician reviewing a colleague

> 💡 Doctor's lesson: a model that is 95% accurate but can't explain itself, fails on a different hospital's X-rays, or is confidently wrong on rare cases is not a clinical tool yet. Evaluation, calibration and bias matter more than the headline number.

## Main resources

- **3Blue1Brown — Neural Networks** (YouTube playlist) https://www.youtube.com/playlist?list=PLZHQObOWTQDNU6R1_67000Dx_ZCJB-3pi
- **fast.ai — Practical Deep Learning** (free) https://www.fast.ai — build first, theory second
- **PyTorch tutorials** https://pytorch.org/tutorials
- **PhysioNet** (medical datasets) https://physionet.org
