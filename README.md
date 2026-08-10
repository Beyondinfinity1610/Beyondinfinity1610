<h1 align="center">Thejeshwaar Sathishkumar</h1>
<h3 align="center">ML Researcher & Signal Engineer — Time-Series, Rare-Event Detection, Bio-Signal & Financial ML</h3>

<p align="center">
Builds and validates ML systems for rare-event detection in noisy, non-stationary time-series — EEG, ECG, and financial transaction data. Two years leading multimodal seizure- and cognitive-state research; currently applying the same methodology to financial event detection in production at a fintech startup.
</p>

<p align="center">
📍 Chennai, India &nbsp;·&nbsp; 🇺🇸 U.S. Citizen &nbsp;·&nbsp;
<a href="mailto:thejeshwaarsathishkumar@gmail.com">✉️ Email</a> &nbsp;·&nbsp;
<a href="https://www.linkedin.com/in/thejeshwaar-sathish-kumar-672a52291">🔗 LinkedIn</a>
</p>

---

### 🧭 What I actually do

Most of my work answers one question: **can a model detect the rare, important event inside a flood of noisy, everyday signal, without lying to itself about how well it's doing?** That question shows up identically whether the signal is a seizure in an EEG trace, a domain shift between two patients' brainwaves, or a life event buried in someone's transaction history. I've built systems that answer it in all three settings, with honest, leakage-free validation every time.

---

### 🔬 Research

**Multimodal Focal-Seizure Detection (NeuroSync)** — *2025–present*
Fused EEG, ECG, EMG, and accelerometer data from a wearable sensor to detect focal seizures in real clinical data (SeizeIT2). Ran a 7-stage ablation campaign that diagnosed and fixed two root-cause failures — including one negative result reported honestly instead of buried.
- **Continuous-stream AUROC 0.826** (9-model selection-free ensemble), **67% sensitivity at 10 false alarms/hr**
- Event-level F1 **8–9× the fair, fully-automated baseline** from a comparable published study
- Every number validated with patient-level, leakage-free splits — no window ever crosses train/test for the same patient

**Domain-Adversarial GNN for EEG Classification** — *2025*
Diagnosed a subject-identity leakage pattern common across EEG-ML literature (models silently memorize *whose* brain they're looking at, not the pathology) and built around it properly.
- Domain-adversarial architecture (gradient-reversal subject classifier) + 5 band-specific graph attention networks over phase-based (wPLI) connectivity, chosen specifically to reject volume-conduction artifacts
- **92.2% accuracy (AUROC 0.946)** on strict leave-one-subject-out validation — up from a ~60% near-chance baseline once leakage is properly removed
- [→ Repository](https://github.com/Beyondinfinity1610/ADHD-CLASSFiCATION-EEG)

**Quantum-Hilbert Hybrid (QHH) Feature Extraction** — *CADS, VIT Chennai, 2025*
Combined Hilbert-transform phase/amplitude preservation with a custom Variational Quantum Circuit to pull structure out of EEG signal beyond classical resolution limits. Manuscript in preparation.
- [→ Repository](https://github.com/Beyondinfinity1610/quantum-hilbert-eeg-feature-learning)

**Financial Time-Series & Event Detection** — *kyfr.ai, 2026*
Same underlying problem as the seizure work, applied to money instead of brainwaves: detecting rare life events (job loss, medical emergency, relocation) inside noisy transaction time-series. Shipped a gradient-boosted + rule + change-point detection ensemble clearing F1 > 0.75 on 3 of 4 target events, served via a production FastAPI/Docker API.

**EEG Motor Imagery Classification (BCI Pipeline)** — *foundational project*
End-to-end pipeline on PhysioNet data — band-pass filtering, ERD feature extraction, Linear SVM — the signal-to-model workflow that everything above builds on.
- [→ Repository](https://github.com/Beyondinfinity1610/EEG-Motor-Imagery-Classification-using-ERD-Features-Beginner-Neuro-AI-Project-)

---

### 🧠 Patents

- **Hardware-Level Self-Healing IoT System** — Patent 202541081235 (Published). Design/IP contribution: fault-detection redundancy architecture targeting sub-50ms sensor-failure response.
- **Distributed Multi-Modal Railway Monitoring (DMQS-EARIMS)** — Patent Pre-Publication. Federated-learning fault-detection design fusing ultrasonic, fiber-optic, and vision sensing.

---

### 🛠️ Technical Toolkit

**Signal & ML** &nbsp;`VMD` `FFT` `Hilbert Transforms` `ERD/ERS` `Multitaper PSD` `PLI/wPLI Functional Connectivity` `Learnable Filterbanks` `Applied DSP`

**Deep Learning** &nbsp;`Rare-Event / Class-Imbalance Detection` `Domain-Adversarial Training (DANN/GRL)` `Graph Attention Networks` `Transformers` `LSTMs/GRUs` `Ensembling` `Variational Quantum Circuits`

**Tools** &nbsp;`PyTorch` `Scikit-Learn` `MNE-Python` `PennyLane` `FastAPI` `Docker` `Python` `MATLAB`

---

### 📫 Reach me

<a href="mailto:thejeshwaarsathishkumar@gmail.com">Email</a> &nbsp;·&nbsp;
<a href="https://www.linkedin.com/in/thejeshwaar-sathish-kumar-672a52291">LinkedIn</a> &nbsp;·&nbsp;
Open to applied ML / signal processing / research roles in the U.S. — bio-signal, communications/RF, and financial time-series.
