# Blood Glucose Prediction with Mixture of Experts Architecture

## Overview
This project aims to predict blood glucose levels in patients using a sophisticated Mixture of Experts (MoE) architecture. The architecture consists of multiple expert models, each specializing in different neural network structures. The goal is to leverage the strengths of various models to achieve a more accurate and robust prediction of blood glucose levels.

## Architecture
The Mixture of Experts architecture employed in this project includes the following components:

* GRU Expert: Utilizes Gated Recurrent Units (GRU) to capture temporal dependencies in blood glucose data.
* LSTM Expert: Employs Long Short-Term Memory (LSTM) networks, known for their ability to learn long-term dependencies, which is crucial for time-series data.
* Dense Layer Expert: Uses a fully connected (Dense) layer network to model the non-linear relationships in the data.

The mixture model combines the outputs of these experts to produce a final prediction. A gating mechanism is used to assign weights to each expert's output based on the input data, allowing the model to dynamically select the most relevant expert(s) for each prediction.
