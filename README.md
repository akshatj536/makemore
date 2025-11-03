# makemore: Character-Level Language Model (Bigram + MLP)

This project is a simplified reimplementation of **Andrej Karpathy’s “makemore”**, which builds a **character-level language model** from scratch. The goal is to understand how modern neural language models, such as GPT, are built up step-by-step, starting from simple statistical models to small neural networks.

---

## 🔹 Overview

The project focuses on generating names (or any short text) one character at a time by learning patterns from a dataset of real names. It explores two key model architectures:

1. **Bigram Model** – The simplest probabilistic model that learns character-to-character transitions directly from data.  
   - It uses counts of character pairs to estimate probabilities of the next character given the previous one.  
   - Despite its simplicity, it captures basic dependencies (like `'q'` often followed by `'u'`).

2. **Multilayer Perceptron (MLP) Model** – A feedforward neural network that extends the bigram idea using learned embeddings and nonlinear transformations.  
   - Characters are encoded as vectors, passed through hidden layers with ReLU activation, and trained using gradient descent.  
   - It learns richer representations and can model more complex dependencies beyond direct character pairs.

---

## 🔹 Key Concepts Covered

- Tokenization and one-hot encoding of characters  
- Data splitting into training, validation, and test sets  
- Log-likelihood loss and model evaluation  
- Backpropagation and gradient updates  
- Comparison between probabilistic and neural approaches  

---

## 🔹 Results

- **Bigram Model**: Produces readable but repetitive names.  
- **MLP Model**: Generates more realistic, diverse, and coherent sequences, demonstrating how neural models improve text generation quality.

---

## 🔹 Purpose

This project is an educational deep dive into how neural text generators evolve from simple statistical rules to neural architectures. It bridges the intuition behind language modeling and the foundational concepts powering large models like GPT.

---

