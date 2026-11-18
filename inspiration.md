# Inspiration — LinkedIn AI-in-medicine links

Saved by Usman in his WhatsApp self-chat, 30 Sep – 15 Oct 2026.
Opened, read and verified 18 Nov 2026.

These are the real projects that shaped this repo's direction. The pattern across
all of them: not just a model — a full product. Train it, explain it (Grad-CAM),
wrap it in an API, deploy it, and make the result lead to a real next step
for the patient. That pattern is what Phases 2–4 of this repo teach.

## Learn AI from scratch

1. **Madhur Mehta — 7 GitHub repos to learn AI from scratch (2026).** Saved 1 Oct 2026.
   Made With ML, Hands-On Large Language Models, Microsoft's Generative AI for
   Beginners, RAG Techniques, AI Agents for Beginners, MCP Servers, AI
   Engineering Hub. The learning roadmap: ML fundamentals → LLMs → GenAI →
   RAG → agents → MCP → real projects.
   https://lnkd.in/p/dNkZEwTC

## Medical imaging AI — real projects

2. **Loai Abdallah — FleXray.** Saved 2 Oct 2026. Universal X-ray segmentation
   model, 60 anatomical structures. Makes synthetic labelled X-rays from
   segmented 3D CT scans plus generative AI, because labelled medical data is
   scarce. Research system, not a clinical tool yet.
   https://www.linkedin.com/posts/loaia_medicalai-medicalimaging-artificialintelligence-ugcPost-7509462481615089665-1tg4

3. **Alaa Ibrahim — RetinaGuard.** Saved 2 Oct 2026. Diabetic retinopathy
   screening from retinal fundus photos. EfficientNet-B0 on APTOS 2019:
   94.6% accuracy, 93.8% sensitivity, 95.4% specificity, AUC 0.982,
   false-negative rate 3.1%. Grad-CAM heatmaps, RAG chatbot (FAISS),
   FastAPI + React + Docker + Nginx, deployed live on a VPS.
   Graduation project, Mashreq University.
   https://www.linkedin.com/posts/alaaibrahim8_artificialintelligence-machinelearning-deeplearning-ugcPost-7510474177620119552-Jpzq

4. **Syeda Sumayya — NeuroScan.** Saved 4 Oct 2026. Brain MRI tumour screening
   (glioma, meningioma, pituitary) with Grad-CAM. The distinctive part: when
   it flags a tumour it points the patient to real neurosurgery and oncology
   hospitals in Pakistan, so the result leads somewhere instead of leaving
   someone stuck with bad news. FastAPI + Next.js, built solo. Research tool,
   not a diagnostic device.
   https://lnkd.in/p/ddK6fQ4x

5. **Atul Shukla — NEUROSCAN AI.** Saved 15 Oct 2026. Also brain MRI tumour
   classification (glioma / meningioma / pituitary / no tumour), PyTorch +
   Grad-CAM, 94.56% accuracy, 0.974 AUC, 96.2% sensitivity, 35 ms inference
   on 1,600 held-out slices. Full app with MRI viewer, report generation,
   live deployment. NOTE: different person, same project name as no. 4 —
   same idea, built independently.
   https://lnkd.in/p/da8qEGtZ

6. **Atria — EchoTrace.** Saved 30 Sep 2026. QLoRA fine-tuning of MedGemma 1.5
   for polygon-based cardiac contouring on echocardiograms: the left
   ventricle border as an editable polygon a cardiologist can drag to correct.
   200/200 valid outputs, median point-to-curve 4.98 mm, Dice 0.744,
   50 held-out patients (CAMUS split), trained in 128 minutes on one GPU.
   Clinician corrections flow back as training labels. The closest of all
   eleven to this repo's LLM direction.
   https://atria.theadimension.com

## Signals — PPG and EEG

7. **Dr. Shresth Gupta — smartphone PPG.** Saved 2 Oct 2026. A phone camera
   reads your pulse: fingertip video → RGB changes → noise removal → PPG
   waveform. Heart rate, pulse-rate variability, cardiovascular dynamics,
   digital biomarkers. Pure CVS physiology + signal processing.
   https://lnkd.in/p/d3uazCwV

8. **A Adith — NeuroLaya.** Saved 2 Oct 2026. EEG cognitive workload
   classification with a fine-tuned Laya model (STEW dataset, 48 subjects,
   14-channel EEG). Subject-disjoint accuracy 66.3%, calibration scores
   reported alongside accuracy. Open source.
   https://lnkd.in/p/dHtXVTju

## Learning tools

9. **Hassan Alhajj — Claude explains MRI.** Saved 2 Oct 2026. Claude Opus 5.5
   built an interactive visual explainer of how an MRI scanner works
   (breast MRI slice acquisition). A teaching tool; the physics details are
   not all verified. Shows what LLMs can build as explainers.
   https://lnkd.in/p/dj3yNp53

10. **Yixiang Wang — NeuroAxis.** Saved 4 Oct 2026. Free interactive 3D
    neuroanatomy learning tool: 3D anatomy synced with 2D sections plus
    clinical context. Built by an ex-Yale neuroanatomy TA with his own
    AI swarm orchestration tool.
    https://lnkd.in/p/dcxufEuE

11. **Yixiang Wang — portfolio.** Saved 4 Oct 2026. Neuroscience PhD, biotech
    veteran, AI builder, 11 projects (learning tools, life sciences,
    personal finance, AI orchestration).
    https://websterwang-ai.github.io

## How they map to this repo

- Phase 0–1 (setup, how LLMs work): no. 1 (the roadmap), no. 6 (MedGemma
  fine-tuning), no. 9 (LLMs as teaching tools).
- Phase 2 (building with LLMs): no. 3 (RAG chatbot pattern), no. 4 and
  no. 5 (FastAPI deployment pattern).
- Phase 3 (evaluation & safety): no. 3 (false negatives matter more than
  accuracy), no. 4 ("a tool that diagnoses the wrong kind of image isn't
  safe"), no. 2 ("research, not clinical yet" honesty).
- Project 2 (ECG classifier): no. 7 (signal processing), no. 8 (signal
  models + calibration).
- As a learner, for revision: no. 10 (anatomy), no. 7 (CVS physiology).

## Learning order — small steps, in this order

1. No. 1, repo 1 (Made With ML) + Phase 0 Python refresh. 15 minutes a day.
2. No. 9 — see what an LLM can build as a teaching tool.
3. No. 3 (RetinaGuard) — study the full-stack pattern: model → explain →
   API → deploy.
4. No. 6 (Atria) — read how MedGemma was fine-tuned; the LLM-for-medical
   endgame.
5. No. 4 / no. 5 — compare the two NeuroScans; same problem, two builds.
6. The rest as interest strikes — no. 2, 7, 8, 10, 11.
