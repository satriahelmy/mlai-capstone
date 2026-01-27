#  Black-Box Optimisation (BBO) Capstone Project

##  Overview
This repository contains the final deliverable for my **Black-Box Optimisation (BBO) Capstone Project**, part of the Professional Certificate in Machine Learning and Artificial Intelligence.  
The project explores how optimisation strategies evolve through iterative experimentation — combining techniques inspired by deep learning, clustering, dimensionality reduction, and reinforcement learning.

Over 13 weeks, the workflow developed from a simple baseline model into an adaptive, feedback-driven optimisation framework capable of learning from its own results and refining its decision-making process.

---

##  Project Objectives
- To design a **dynamic surrogate model** that approximates unknown black-box functions.  
- To balance **exploration and exploitation** through adaptive learning.  
- To iteratively refine queries based on feedback, visualisation, and interpretability.  
- To document the entire process transparently for both technical and non-technical audiences.

---

##  Methodology Overview
The project followed an **iterative optimisation loop**. Each week introduced new techniques to improve accuracy, robustness, and interpretability.

| Week | Focus Area | Key Technique | Summary |
|------|-------------|---------------|----------|
| 1–4 | Baseline Setup | Random Search + MLP Surrogate | Established input/output parsing, model pipeline, and random query sampling. |
| 5–6 | CNN-inspired Deep Learning | Multi-layer MLP (256-128-64-32) | Captured non-linear dependencies; improved accuracy and representation depth. |
| 7–8 | Hyperparameter Tuning | Grid Search & Bayesian Optimisation | Balanced overfitting vs generalisation; optimised architecture and learning rate. |
| 9–10 | LLM-inspired Transparency | Datasheet + Model Card Documentation | Integrated interpretability, model ethics, and reproducibility. |
| 11 | Clustering Analysis | K-Means + Silhouette Evaluation | Identified recurring query clusters; improved sampling diversity. |
| 12 | PCA Decomposition | Dimensionality Reduction | Revealed variance structure; simplified high-dimensional data spaces. |
| 13 | Reinforcement Learning | Adaptive Exploration Bonus | Introduced reward-driven exploration; optimised convergence and robustness. |

---

##  Results and Visual Insights
The final model demonstrated stable predictions across all eight unknown functions.  
- Reinforcement-driven exploration improved the **diversity of sampled regions**.  
- PCA and clustering clarified **patterns and redundancy** in the search space.  
- The **Actual vs Predicted plots** across weeks showed clear convergence trends.  
- Adaptive learning yielded consistent improvement in function approximation.


## Technical Highlights
- **Language:** Python (NumPy, scikit-learn, matplotlib, seaborn)  
- **Model:** `MLPRegressor` wrapped in a `Pipeline` with `StandardScaler`  
- **Optimisation logic:** Reinforcement bonus added to surrogate predictions  
- **Dimensional insights:** PCA used for variance analysis (Week 12)  
- **Clustering:** K-Means used to evaluate pattern groupings (Week 11)  
- **Data management:** Iterative weekly structure (`/weekX_inputs.npy`, `/weekX_outputs.npy`)  
- **Documentation:** Datasheet and Model Card included for transparency  

---

##  Key Learnings
- Optimisation is not just about finding the best value — it is about **designing a learning process** that can improve itself.  
- Reinforcement learning concepts can successfully balance **risk-taking (exploration)** and **stability (exploitation)** in iterative models.  
- Interpretability through PCA, clustering, and visual tracking increases **trust and understanding** of black-box systems.  
- Maintaining **modularity, documentation, and reproducibility** transforms academic experiments into professional-grade ML artefacts.

---

##  Reflection Summary
Over the course of the project:
- The model evolved from a static predictor into a **self-improving adaptive system**.  
- CNN-inspired depth improved expressive capacity.  
- PCA simplified structure and increased interpretability.  
- RL-inspired exploration introduced autonomy and adaptability.  
- The final phase balanced *precision, transparency, and learning efficiency*.  

---

## Documentation
- [Datasheet for BBO Dataset](./datasheet.md)
- [Model Card for BBO Surrogate Model](./model_card.md)
