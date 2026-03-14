# Experiments

This folder contains the Jupyter notebooks used to run the experiments for the thesis project on **crowd anomaly detection using synthetic data**.

The experiments evaluate the impact of adding synthetic data to the training process of the **ASTNet detector**, using different real/synthetic data ratios and selection strategies.

## Training and Testing Protocol

Two datasets are used in the experiments:

- **Ped2 dataset** (real-world surveillance dataset)
- **Synthetic dataset** generated for research purposes

### Training
Training is performed using:

- **Ped2 dataset**
- **Synthetic dataset**

Different experiments explore multiple combinations of real and synthetic data.

### Testing

Two evaluation settings are considered:

- **Intra-dataset evaluation**  
  The model is trained on Ped2 (or Ped2 + synthetic data) and tested on **Ped2**.

- **Cross-dataset evaluation**  
  The model is tested on the **MED dataset** in order to evaluate the **generalization capability** of the trained models.

The MED dataset contains **31 videos (~45,000 frames)** and is used only for evaluation.

---

## Experiment Overview

| Notebook | Description |
|--------|-------------|
| **0-Baseline_pretrain_with_ped2.ipynb** | Baseline experiment using Ped2 data with pretrained weights. |
| **1_train_ped2.ipynb** | Training using only the Ped2 dataset. |
| **2-train_with_synth.ipynb** | Training using only synthetic data. |
| **3-train_50ped2_50synth.ipynb** | Training with 50% real Ped2 data and 50% synthetic data (manual selection). |
| **4-train_75ped2_25synth.ipynb** | Training with 75% real Ped2 data and 25% synthetic data (manual selection). |
| **5-train_90ped2_10synth.ipynb** | Training with 90% real Ped2 data and 10% synthetic data (manual selection). |
| **6-train_random_50ped2_50synth.ipynb** | Training with 50% real Ped2 data and 50% synthetic data (random selection). |
| **7-train_random_75ped2_25synth.ipynb** | Training with 75% real Ped2 data and 25% synthetic data (random selection). |
| **8-train_random_90ped2_10synth.ipynb** | Training with 90% real Ped2 data and 10% synthetic data (random selection). |

---

## Notes

- All experiments use the **ASTNet implementation** available in the repository fork.
