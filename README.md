# LEAF Customization for Federated Learning Experiments

This repository is a fork of [LEAF](https://github.com/TalwalkarLab/leaf), designed to explore and address the challenges posed by heterogeneity in Federated Learning environments.

## Overview

Federated Learning (FL) introduces complex challenges due to the heterogeneity of participants, including variations in device capabilities, data distributions, and participant behaviors. This fork extends the functionality of LEAF to simulate and analyze these challenges, focusing on their impact on model performance, convergence, and fairness.

## Methodology

The modifications implemented in this repository include:

1. **Heterogeneity Simulation**:
   - Adjusted configurations to represent varying device capabilities (e.g., processing power, energy constraints, and network conditions).
   - Introduced models for simulating non-IID data distributions across participants.


3. **Algorithmic Adjustments**:
   - Evaluated advanced aggregation strategies to mitigate the effects of stragglers and system delays.
   - Tested parameter tuning techniques to optimize performance in heterogeneous settings.

3. **Performance Analysis**:
   - Conducted experiments to measure the impact of heterogeneity on metrics such as model accuracy, convergence time, and resource utilization.
   - Analyzed the results to propose potential solutions for enhancing Federated Learning in real-world scenarios.

### Experimental Setup

The experiments were conducted using the FEMNIST dataset and a Federated Learning setup under two different data distributions: IID and non-IID. The specific configurations were:

- **Dataset**: FEMNIST (Federated Extended MNIST)
- **Model**: 2-layer Convolutional Neural Network (CNN)
- **Aggregation Method**: FedAvg
- **Number of Clients**: 50
- **Training Rounds**: 200
- **Train-Test Split**: 80%-20%



## Results Summary

1. **Non-IID Scenario**:
   - Mean Train Accuracy: **0.82**
   - Accuracy Percentiles:
     - 10th: **0.65**
     - 50th: **0.83**
     - 90th: **0.94**
   - Observed heterogeneity in client performance due to data and system differences.

2. **IID Scenario**:
   - Mean Train Accuracy: **0.84**
   - Accuracy Percentiles:
     - 10th: **0.74**
     - 50th: **0.84**
     - 90th: **0.91**
   - Reduced variability in client performance compared to the non-IID case.

These results highlight the significant impact of heterogeneity on Federated Learning performance and the need for adaptive strategies to mitigate its effects.

## Applications

This fork provides a foundation for researchers to:
- Study the impact of heterogeneity on Federated Learning models.
- Develop and test strategies to mitigate heterogeneity-related challenges.
- Enhance the robustness and scalability of FL systems in diverse environments.

## Acknowledgments

This project is based on the LEAF framework and extends its capabilities to address heterogeneity in Federated Learning, special thanks to the original developers of LEAF and the research community for their contributions to this field.

## License

This project inherits the original LEAF [MIT License](https://opensource.org/licenses/MIT).

