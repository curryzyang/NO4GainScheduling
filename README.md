# NO-Event-Triggering Gain Scheduling

Event-triggered gain scheduling simulations with neural-operator experiments for hyperbolic PDEs. This repository contains the main Lyapunov-based ETC simulation notebook, training/analysis notebooks for kernel data, and a pre-trained model.

## Contents

- ETC-Lyapunov-Simulation.ipynb: main Lyapunov-based ETC simulation and visualization.
- ETC_NO_TrainData_AllKernels.ipynb: kernel data generation for training.
- ETC_NO_AllKernle_unaligend.ipynb: neural-operator training and evaluation.
- ETC_NO_AllKernle_unaligend_witherror.ipynb: neural-operator with triggering condition related to approximation error.
- neural_operator_etc_model.pt: saved model weights.

## Setup

1. Create a Python environment (3.9+ recommended).
2. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

## Usage

- Open and run ETC-Lyapunov-Simulation.ipynb for the main simulation.
- Use ETC_NO_TrainData_AllKernels.ipynb to generate kernel data.
- Use ETC_NO_AllKernle_unaligend.ipynb to train/evaluate the neural operator.
- Use ETC_NO_AllKernle_unaligend_witherror.ipynb to train the neural operator with approximation error.

## Outputs

The notebooks save plots inline and may write artifacts such as:
- etc_lyapunov_simulation_results.npz

## Notes

- Some notebooks can be compute-intensive (kernel solvers and training). Consider reducing grid sizes or time horizons for quick tests.
- The model file is provided as a reference artifact; retraining may require GPU for reasonable runtime.
