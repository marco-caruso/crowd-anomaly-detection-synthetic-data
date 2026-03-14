# Experiments

This folder contains the Jupyter notebooks used to run and analyze the experiments presented in the thesis.

The experiments evaluate the impact of synthetic data on cross-dataset training for crowd anomaly detection using the ASTNet detector.

Each notebook corresponds to a specific training configuration and dataset composition.

## Experiment Overview

| Notebook | Description |
|--------|-------------|
| 
| 01_baseline.ipynb | Training and testing using only the Ped2 dataset |
| 02_ped2_synth_50_manual.ipynb | Training with 50% real data and 50% synthetic data (manual selection) |
| 03_ped2_synth_75_manual.ipynb | Training with 75% real data and 25% synthetic data (manual selection) |
| 04_ped2_synth_90_manual.ipynb | Training with 90% real data and 10% synthetic data (manual selection) |
| 05_ped2_synth_50_random.ipynb | Training with 50% real data and 50% synthetic data (random selection) |
| 06_ped2_synth_75_random.ipynb | Training with 75% real data and 25% synthetic data (random selection) |
| 07_synthetic_only.ipynb | Training using only synthetic data |
| 08_med_test.ipynb | Cross-dataset evaluation on the MED dataset |

## Notes

- All experiments use the ASTNet detector implementation.
- The configuration files used for training are available in the ASTNet fork.
- Pretrained model checkpoints can be downloaded from the provided Google Drive link in the main repository README.
