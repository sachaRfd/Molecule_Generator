# LSTM Molecule Generator

#### Proof Of Concept with Notebook only

## Overview

The LSTM Molecule Generator is a project aimed at utilizing Recurrent Neural Networks (RNNs), specifically Long Short-Term Memory (LSTM) networks, to generate novel and theoretically feasible chemical compounds in SMILES (Simplified Molecular Input Line Entry System) format. SMILES is a widely used string-based representation of chemical structures.

The primary goal of this project is to train an LSTM-based model to learn the underlying patterns and relationships within chemical compounds and then generate new, diverse compounds that adhere to chemical validity. LSTMs have shown promising results in generating SMILES strings (as demonstrated in [this study](https://doi.org/10.1186/s13321-019-0393-0)), making them a suitable choice for this task.

## Project Details

The project involves the following steps:

1. **Data Collection**: The project begins with the acquisition of chemical compound data in SMILES format. The data will be obtained from the ZINC database, a reliable source for such information. The data can be downloaded from the following URL: [ZINC Chemical Compound Data](http://files.docking.org/2D/).

2. **Data Preprocessing**: The acquired SMILES data will undergo preprocessing to ensure its quality and consistency. This step involves tasks such as data cleaning, tokenization, and sequence padding, preparing the data for model training.

3. **Model Architecture**: The core of the project is the design and implementation of the LSTM-based neural network. The LSTM architecture will be configured to learn the sequential patterns in the SMILES data. Model hyperparameters, layer configurations, and optimization strategies will be fine-tuned to achieve optimal performance.

4. **Training and Validation**: The model will be trained on the preprocessed data, and its performance will be evaluated using validation techniques. Training progress and performance metrics will be monitored to prevent overfitting and ensure convergence.

5. **Generation of New Compounds**: Once the LSTM model is trained and validated, it will be utilized to generate new SMILES strings representing novel chemical compounds. The generation process can be controlled using temperature settings, allowing for the exploration of compounds with varying degrees of complexity.

## Results

The project aims to achieve the following outcomes:

- Successful implementation of an LSTM-based RNN for generating new SMILES strings of chemical compounds.
- Generation of diverse and theoretically feasible chemical compounds by adjusting the temperature settings of the LSTM model.
- Exploration of the generated compounds to identify novel and potentially interesting chemical structures.

## Usage

To replicate and contribute to this project, follow these steps:

1. Download the SMILES data from [ZINC](http://files.docking.org/2D/) and save it in the appropriate data directory.
2. Configure the LSTM model architecture and generate new smiles strings within minutes in the provided notebook (`LSTM_Molecule_Generator.ipynb`) varying the temperature settings for different levels of complexity

## References

- [Original LSTM SMILES Generation Study](https://doi.org/10.1186/s13321-019-0393-0)
- [ZINC Database for Chemical Compounds](http://files.docking.org/2D/)

Feel free to contribute, provide feedback, or explore new avenues for enhancing the LSTM Molecule Generator project!
