# Datasheet for BBO Capstone Project Dataset

## Motivation
This dataset was created to support a Black-Box Optimization (BBO) capstone project as part of Stage 2.  
It contains query–response pairs across eight unknown mathematical functions, used to train surrogate models and refine optimization strategies over 10 weeks.  
The goal is to enable transparent benchmarking of model-driven query selection techniques.

## Composition
- **Instances:** 19 data points per function (8 total functions)
- **Features:** Normalized inputs (x₁, x₂, …, xₙ) where n = 2–8 depending on function
- **Outputs:** Observed scalar function responses (y)
- **Format:** Stored as `.npy` (NumPy arrays) and plain text (`inputs.txt`, `outputs.txt`)
- **Gaps:** Some sparse high-dimensional regions remain underexplored.

## Collection Process
Queries were generated weekly by a trained surrogate model (MLP/CNN-based), with one query per function per round.  
Each iteration refined based on prior performance and model prediction uncertainty.  
Data collection occurred across ten rounds over approximately 10 weeks.

## Preprocessing & Uses
Minimal preprocessing applied. Values normalized to [0, 1] for input domains.  
Intended use includes surrogate modeling, regression analysis, and exploration of optimization behavior.  
Inappropriate uses include attribution of physical meaning or external deployment beyond simulation scope.

## Distribution & Maintenance
The dataset is maintained under the student’s GitHub repository for academic use only.  
Terms of use: Open for peer review within the course. Not for commercial distribution.
Maintainer: [Your Name] (Imperial College London BBO Capstone Participant)
