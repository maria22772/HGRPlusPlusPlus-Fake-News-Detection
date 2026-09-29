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

Contains the additional binary fake-news evaluation using the GossipCop dataset from FakeNewsNet. The notebook includes image validation, stratified train/validation/test splitting, HGR+++ training, and final evaluation.

## Datasets

The primary experiments use the **Fakeddit** multimodal fake-news dataset.

The additional evaluation uses **GossipCop** from the **FakeNewsNet** dataset.

The original third-party datasets and raw images are not redistributed in this repository. Users should obtain the datasets from their respective original sources.

## Execution Environment

The experiments were conducted using **Kaggle notebooks** with GPU acceleration.

For reproducibility, the notebooks retain the Kaggle input paths used during the original experiments. Users reproducing the experiments on Kaggle should attach the corresponding datasets and use the appropriate input paths. Users running the code in another environment may need to modify the dataset path variables.

## Reproducibility

The notebooks document the experimental workflow used in the study, including:

- dataset preparation and preprocessing
- multimodal feature processing
- HGR+++ model implementation
- training configuration
- evaluation procedures
- metadata-related analyses
- leakage and near-duplicate sensitivity analyses
- additional GossipCop evaluation

Random seeds and major training hyperparameters are specified directly in the notebooks where applicable.

## HGR+++

HGR+++ stands for **Hierarchical Gated Residual Fusion**.

The model combines CLIP-based text and image representations with contextual information through a context-conditioned gating mechanism and centered residual fusion for multimodal fake-news classification.

## Code Availability

The notebooks in this repository are provided to support reproducibility of the experiments and analyses reported in the manuscript.

## Citation

If you use this repository, please cite the associated manuscript.

Full citation information will be added after publication.
