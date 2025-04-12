# Comparative Analysis of Transformer and MLP for Sequence Prediction

## Group Members
- Dejina Ghale (200582110)  
- Shishir Aryal (200582212)

---------------------------------------
## How to Run

1. Clone this repository  
2. Make sure Python and PyTorch are installed  
3. Open `Updated_Transformer.ipynb` in Jupyter Notebook or VS Code  
4. Run all cells to train and compare the models

## Overview

This project compares a Transformer model and a simple Multi-Layer Perceptron (MLP) on a sequence prediction task using synthetic data. The goal was to see how well each model could learn to approximate a sigmoid function.

We were inspired by the paper *"Large Scale Legal Text Classification Using Transformer Models"*, and adapted a similar Transformer architecture to this toy problem.

-------------

## Models

### MLP
- Simple 2-layer model
- Uses ReLU activation
- Takes a flattened input sequence
- Predicts a single output value (regression)

### Transformer
- Custom implementation using PyTorch
- Includes multi-head self-attention
- Uses embeddings and positional encodings
- Designed for sequence-to-sequence prediction

---

## Tools and Libraries
- Python  
- PyTorch  
- Jupyter Notebook  
- Matplotlib (for plots and loss curves)


--------------------------------------
## Results

- The MLP model had a final loss of 0.97 and trained faster with smoother results.
- The Transformer model had a final loss of 1.05 and trained slower with more ups and downs

- The MLP performed better for this simple task.

- The Transformer still captured the shape of the sigmoid function reasonably well.

-----------------------------

## Visualizations
- Loss curves for both models
- Sigmoid vs Transformer output comparison
- Epoch-wise loss tracking

--------------------------------------------------------------------

## Key Observations
- MLPs are efficient and reliable for simple problems.
- Transformers are more powerful but require more data and tuning.
- Visual feedback was helpful in understanding model performance.

---------------------------------

## Limitations
- Only tested on synthetic data.
- No real-world datasets were used.
- No pretraining or hyperparameter tuning was done.

------------------------------------

## Future Work
- Try real-world datasets like EUR-Lex or JRC-Acquis
- Use pretrained Transformer models like BERT or Longformer
- Add noise or imbalance to data to test robustness
- Compare with other models like CNNs or LSTMs

---



---------------------------------------

## Reference

Paper: *Large Scale Legal Text Classification Using Transformer Models*  
Link: https://paperswithcode.com/paper/large-scale-legal-text-classification-using
