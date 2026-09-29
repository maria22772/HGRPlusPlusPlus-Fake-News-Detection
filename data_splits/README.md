# Dataset Split Information

This directory contains the train, validation, and test split information used in the experiments reported in the manuscript.

For Fakeddit, the provided split files correspond to the final 99,200 training, 12,400 validation, and 12,400 test samples used in the main experiments.

For GossipCop, the additional evaluation used 8,302 multimodal samples with a stratified partition of 6,641 training, 830 validation, and 831 test samples. The experimental partitioning is defined programmatically in `03_gossipcop_additional_evaluation.ipynb` using a fixed random seed.

The original Fakeddit and GossipCop datasets and associated images are not redistributed in this repository. They should be obtained from their respective original sources.

The complete cleaned GossipCop dataset is not included because of its large file size and third-party dataset origin.

The Fakeddit split files provided here document the exact experimental partitions used in the main experiments and are intended to support reproducibility.
