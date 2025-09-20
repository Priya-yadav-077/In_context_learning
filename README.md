# Transformers Learn In-Context by Gradient Descent

## A Study on the Impact of Attention Mechanisms and Architectural Depth on In-Context Learning

### **Project Overview**

This repository contains the code and results for the project report "A Study on the Impact of Attention Mechanisms and Architectural Depth on In-Context Learning," submitted for the course "The Mystery Of In-Context Learning Of Large Language Models" at the University of Heidelberg.

Building upon the foundational research of Von Oswald et al. (2022), this study investigates the architectural parameters that impact a transformer's ability to learn an in-context gradient descent task. The primary focus of this research is to systematically examine the influence of two critical architectural choices: the attention mechanism and network depth, on the model's performance and training stability.

### **Repository Contents**

* `experiment_setup.ipynb`: This Jupyter notebook contains the complete, reproducible code used to run all experiments described in the project report. It allows for the replication of the baseline and all six phases of the study.


### **Key Findings**

The research presented here demonstrates several key conclusions:

1.  **Attention Mechanism:** The softmax attention mechanism is crucial for the transformer's ability to perform in-context learning. Models without this mechanism consistently failed to converge.
2.  **Network Depth:** Increasing network depth systematically improves the model's performance up to a certain point, with the 8-layer network achieving the lowest loss on a more complex problem.
3.  **Scaling Limit:** A critical finding is the existence of a scaling limit. The 16-layer model exhibited catastrophic failure due to gradient explosion, highlighting the inherent instability of deep neural networks in this specific task and the need for careful regularization.

This repository serves as a complete record of the research, providing full transparency and the necessary resources for reproducibility.
