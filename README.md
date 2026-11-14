# xai-class-imbalance-study
# Disagreement and Faithfulness of TreeSHAP and LIME under Class Imbalance

## Project Overview

This project investigates how class-imbalance handling strategies influence the agreement and faithfulness of TreeSHAP and LIME explanations in credit default prediction.

## Research Question

Does the choice of class-imbalance handling strategy affect feature-level agreement, rank agreement, sign agreement, and explanation faithfulness between TreeSHAP and LIME?

## Dataset

UCI Default of Credit Card Clients Dataset.

- 30,000 instances
- 23 predictive features
- Binary classification task

## Experimental Configuration

- Model: Random Forest (100 estimators)
- Training prevalences: 22%, 15%, 10%, 5%, 2%
- Strategies: Unweighted, Balanced-subsample, SMOTE
- Repeated stratified splits: 5
- Explainability methods: TreeSHAP and LIME
- Faithfulness metric: AOPC

## Evaluation Metrics

- ROC-AUC
- PR-AUC
- F1-score
- Feature Agreement (FA)
- Rank Agreement (RA)
- Sign Agreement (SA)
- Area Over the Perturbation Curve (AOPC)

## Repository Structure

- `notebooks/`: Experimental notebook
- `results/`: Experimental outputs
- `figures/`: Generated plots
- `report/`: LaTeX source and PDF report

## Reproducibility

The experiments use controlled random seeds and five stratified train-test splits. Refer to the notebook and configuration files for the complete experimental procedure and execution instructions.

## AI Tool Usage Disclosure

AI tools were used for supporting code debugging, conceptual clarification, and report preparation. All experimental configurations, code, and results were reviewed by the project team.

## Authors

Fathimath Anshifa Sherin A  
Sri Shakthi Sarath Chintapalli
