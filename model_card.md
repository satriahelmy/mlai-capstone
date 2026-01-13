# 🧠 Model Card for BBO Optimization Surrogate

## Overview
- **Model Name:** Week10 Transparent Surrogate (MLP-based)
- **Version:** 1.0 (Final BBO Stage 2 submission)
- **Frameworks:** scikit-learn, NumPy, Matplotlib

## Intended Use
Designed for experimental optimization in a black-box setting.  
Suitable for comparing neural surrogate–based search methods.  
Not intended for production or deployment on sensitive real-world tasks.

## Details
The model uses a fully connected MLP with layer sizes (512, 256, 128), `ReLU` activations, and `Adam` optimizer.  
It predicts function responses from query coordinates, then selects new candidates with the highest predicted score.  
Transparency is ensured by automatically logging top-5 candidate predictions, confidence trends, and plots for each function.

## Performance Summary
Across eight unknown functions:
- Mean R² on training data ≈ 0.97  
- Typical output ranges: [-33, 4400]  
- Query prediction accuracy improved progressively up to Week 10  
Each round contributes to refined sampling, minimizing redundant queries.

## Assumptions & Limitations
Assumes local smoothness in response surface.  
Limitations include overfitting on small data and interpretability trade-offs due to deep architectures.

## Ethical Considerations
All experiments are conducted on synthetic functions, with no personal data or sensitive content involved.  
Transparency practices (auto-logging, plots, reproducible configs) ensure interpretability and reproducibility in academic evaluation.
