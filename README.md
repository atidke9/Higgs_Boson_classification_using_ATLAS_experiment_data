**Objective**: To classify simulated particle collision events as either signals (indicating the decay of a Higgs boson) or background noise, using LSTM models to process features derived from these events.

**Data**: The analysis is based on simulated data from the ATLAS experiment at the Large Hadron Collider (LHC), CERN.

**Motivation**: To bridge the gap between theoretical knowledge of Recurrent Neural Networks (RNNs) and practical application in particle physics.

**Methodology**:

*Data Cleaning*:

Remove redundant features.
Handle missing values.
Normalize data for uniformity.

*Feature Engineering*: Use both primitive (raw detector readings) and derived (calculated from primitives) features.

*Model Architecture*: Develop an LSTM model architecture to process time-series data.

*Initial Attempt*: Started with a batch size of 16, but faced large loss values and low accuracy.

*Iterative Experimentation*:

Conducted experiments varying batch sizes and monitoring different performance metrics.
Best validation accuracy obtained:
75.86% with both primitive and derived features.
75.60% with derived features.
71.51% with primitive features.

*Optimized Approach*:

Derived features provided the best balance between computational efficiency and model performance.
Slight accuracy trade-off for reduced computational cost and feature count. 

**Conclusion**: 

The second experiment, focusing on derived features, deemed most effective.
Achieved a competitive validation accuracy with fewer features and less computational demand
