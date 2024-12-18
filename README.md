# Learning Cortico-Muscular Dependence through Orthonormal Decomposition of Density Ratios 

## Overview
Welcome to the GitHub repository for our paper *Learning Cortico-Muscular Dependence through Orthonormal Decomposition of Density Ratios*. Here, you will find datasets, models, and codes for training and visualization as described in the paper. 🧠💪

## Contents
The repository is structured with notebook files for training and visualization, organized as follows:

- **1.1. Preprocessing** ✅ 
- **2.1 Main Experiment - Inter Subject Experiments** ✅ 
- **2.2 Main Experiment - Cross Subject Experiments** ✅ 
- **3.1 Visualization - Span of Eigenfunctions** ✅ 
- **3.2 Visualization - Temporal Channel Dependence** ✅ 
- **4.1 Baseline - CMC** ✅ 
- **4.2 Baseline - MI** ✅ 

## Getting Started

### 1. Preprocessing
#### Downloadable Files:
- **Raw Data**: https://doi.org/10.1093/gigascience/giaa098
- **Filtered EEG/EMG Numpy Arrays**: https://drive.google.com/drive/folders/1e0nqKcb7MoAJQd4aaEAfbvKjzURMVkyH?usp=sharing
- **Trained Models**: 

#### Processing Steps:
1. Download the necessary raw data files: `eeg_train_trial.pt`, `emg_filtered_train_trial.pt`, `label_train_trial.pt`, `sub_train_trial.pt`, and update the paths accordingly.
2. Execute the blocks in `Preprocessing.ipynb` to save filtered signals (outliers removed) and primary movement labels as numpy arrays.

### 2. Running Experiments
#### Inter Subject Experiments:
1. After preprocessing, execute the **Inter Subject Experiments** notebook section by section.
2. This will store the trained models and learning curves locally.
3. **Note**: Inter Subject is used for visualizations and must be run before visualization.

#### Cross Subject Experiments:
1. Running the **Cross Subject Experiments** notebook will save the highest accuracies during training.

### 3. Visualization
#### Span of Eigenfunctions:
1. Load the trained models and extract training and testing set features for both EEG and EMG data.
2. Use EEG features for visualizations.

##### Produced Figures:
- Projection of all samples, color-coded by subject index and movement types.
- Specific projections of individual subjects and their movements.
- Approximated density ratios values.

#### Temporal-Level and Channel-Level Dependencies:
1. Use the saved model from **Inter Subject Experiments (2.1)**.
2. Produce temporal-level and channel-level dependencies figures.

### 4. Baseline:
- Contains codes for **CMC** and **MINE**.

Happy Experimenting! 
