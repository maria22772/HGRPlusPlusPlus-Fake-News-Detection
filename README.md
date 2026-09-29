# HGR+++: Metadata-Conditioned Hierarchical Gated Residual Fusion for Fine-Grained Multimodal Fake News Detection

This repository contains the implementation and reproducibility materials for the manuscript:

**“HGR+++: Metadata-Conditioned Hierarchical Gated Residual Fusion for Fine-Grained Multimodal Fake News Detection”**

The repository includes the main Fakeddit experiments, additional verification and sensitivity analyses conducted during manuscript revision, and the additional GossipCop evaluation.

## Repository Contents

### 1. Main Fakeddit Experiments

**`01_fakeddit_main_experiments.ipynb`**

Contains the primary experimental pipeline used for the Fakeddit experiments, including data preparation, HGR+++ training, evaluation, and generation of the main experimental results.

### 2. Fakeddit Revision and Verification Experiments

**`02_fakeddit_revision_verification.ipynb`**

Contains additional experiments and verification analyses performed during manuscript revision, including:

- metadata dependency and shortcut/artifact analysis
- controlled metadata ablations
- cross-split overlap checks
- text-similarity analysis
- near-duplicate sensitivity analysis
- additional reproducibility and robustness checks

### 3. Additional GossipCop Evaluation

**`03_gossipcop_additional_evaluation.ipynb`**

Contains the additional binary fake-news evaluation using the GossipCop dataset from FakeNewsNet, including experimental data handling, stratified train/validation/test splitting, HGR+++ training, and final evaluation.

## Datasets

The primary experiments use the **Fakeddit** multimodal fake-news dataset.

The additional evaluation uses **GossipCop** from the **FakeNewsNet** dataset.

The `data_splits/` directory provides the experimental split information corresponding to the experiments reported in the manuscript.

For Fakeddit, the final experimental splits contain:

- Training: 99,200 samples
- Validation: 12,400 samples
- Test: 12,400 samples

For GossipCop, the experimental splits contain:

- Training: 6,641 samples
- Validation: 830 samples
- Test: 831 samples

The original third-party datasets and associated images are not redistributed in this repository. Users should obtain the datasets from their respective original sources.

## Execution Environment

The experiments were conducted using **Kaggle notebooks** with GPU acceleration.

For reproducibility, the notebooks retain the Kaggle input paths used during the original experiments. Users reproducing the experiments on Kaggle should attach the corresponding datasets and use the appropriate input paths. Users running the code in another environment may need to modify the dataset path variables.

## Reproducibility

The repository documents the experimental workflow used in the study, including:

- Fakeddit data preparation and experimental split construction
- multimodal feature processing
- HGR+++ model implementation
- training configuration
- evaluation procedures
- metadata-related analyses
- leakage and near-duplicate sensitivity analyses
- GossipCop experimental split construction
- additional GossipCop training and evaluation

Random seeds and major training hyperparameters are specified directly in the notebooks where applicable.

The `data_splits/` directory provides the split information corresponding to the experiments reported in the manuscript.

## HGR+++

HGR+++ stands for **Hierarchical Gated Residual Fusion**.

The model combines CLIP-based text and image representations with contextual information through a context-conditioned gating mechanism and centered residual fusion for multimodal fake-news classification.

## Code Availability

The notebooks and experimental split information provided in this repository are intended to support reproducibility of the experiments and analyses reported in the manuscript.

## Citation

If you use this repository, please cite the associated manuscript.

Full citation information will be added after publication.
