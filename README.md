
<div align="center">

# 🧠 Neural Network Lab

### Understand the Mathematics Behind Deep Learning

An interactive educational laboratory for Neural Networks, Deep Learning and Neural Language Models.

![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![SVG](https://img.shields.io/badge/SVG-FFB13B?style=for-the-badge&logo=svg&logoColor=black)
![GitHub Pages](https://img.shields.io/badge/GitHub_Pages-222222?style=for-the-badge&logo=github)

![Lessons](https://img.shields.io/badge/Interactive_Lessons-23-0D9488?style=flat-square)
![Review](https://img.shields.io/badge/Review_Questions-10-6366F1?style=flat-square)
![Dependencies](https://img.shields.io/badge/JS_Frameworks-None-22C55E?style=flat-square)
![Learning](https://img.shields.io/badge/Learning-Simulation_Based-E76F51?style=flat-square)

<br>

### [🚀 Launch Interactive Lab](https://arafat-rahman-lisan.github.io/neural-network-simulation/)

[Overview](#overview) • [Visual Showcase](#visual-showcase) • [Curriculum](#learning-curriculum) • [Architecture](#system-architecture)

<br>

<img src="./screencapture-arafat-rahman-lisan-github-io-neural-network-simulation-2026-11-25-01_37_07.png" width="95%" alt="Neural Network Lab">

*Don't just memorize neural networks. Understand how they work.*

</div>

---

## Overview

Neural Network Lab transforms theoretical deep learning and NLP concepts into interactive mathematical experiments.

Instead of relying exclusively on static lecture slides and equations, the platform allows learners to manipulate weights, biases, activation functions and network parameters while observing their effects in real time.

The project contains 23 structured lessons, progressing from a single computational neuron to feedforward neural networks, language models, gradient descent and backpropagation.

| 23 Lessons | 9 Learning Modules | 10 Review Questions |
|:---:|:---:|:---:|
| Interactive curriculum | Progressive mathematical concepts | Self-assessment |

---

## Visual Showcase

### 01 · Neural Network Signal Propagation

<div align="center">

<img src="./screencapture-arafat-rahman-lisan-github-io-neural-network-simulation-2026-11-25-01_37_07.png" width="95%" alt="Neural signal propagation">

</div>

Explore how information travels through input, hidden and output layers.

- Animated neural signal propagation
- Feedforward network representation
- Interactive network diagrams
- Conceptual explanation of hidden layers
- Comparison with logistic regression

---

### 02 · Activation Function Playground

<div align="center">

<img src="./screencapture-arafat-rahman-lisan-github-io-neural-network-simulation-2026-11-25-01_36_14.png" width="95%" alt="Interactive sigmoid function">

</div>

Experiment with activation functions and observe how numerical inputs are transformed into nonlinear outputs.

- Adjustable input values
- Real-time sigmoid calculations
- Interactive mathematical curves
- Step-by-step numerical substitution
- Sigmoid, tanh and ReLU comparisons

The fundamental computation:

$$
z = \mathbf{w}^{T}\mathbf{x}+b
$$

$$
\sigma(z)=\frac{1}{1+e^{-z}}
$$

---

### 03 · Vanishing Gradient Simulation

<div align="center">

<img src="./screencapture-arafat-rahman-lisan-github-io-neural-network-simulation-2026-11-25-01_37_19.png" width="95%" alt="Vanishing gradient simulation">

</div>

Visualize how gradients become progressively smaller as they travel backward through a deep neural network.

| Interactive Parameter | Purpose |
|---|---|
| Network depth | Adjust the number of layers |
| Activation magnitude | Explore saturation effects |
| Activation type | Compare sigmoid and ReLU |
| Gradient strength | Observe signal decay layer by layer |

The simulation illustrates repeated multiplication of local derivatives in a simplified backpropagation scenario.

$$
g_{\text{early}} = g_{\text{late}}
\prod_{i=1}^{n} f'(z_i)
$$

When derivatives repeatedly take values much smaller than one, gradients can become extremely small.

---

### 04 · Perceptron and XOR Classification

<div align="center">

<img src="./screencapture-arafat-rahman-lisan-github-io-neural-network-simulation-2026-11-25-01_37_34.png" width="95%" alt="Perceptron decision boundary">

</div>

Investigate why a single perceptron can classify AND and OR but cannot represent XOR.

- Interactive AND, OR and XOR datasets
- Adjustable weights and bias
- Real-time decision boundary visualization
- Classification accuracy feedback
- Multilayer ReLU solution for XOR

| Input 1 | Input 2 | AND | OR | XOR |
|:---:|:---:|:---:|:---:|:---:|
| 0 | 0 | 0 | 0 | 0 |
| 0 | 1 | 0 | 1 | 1 |
| 1 | 0 | 0 | 1 | 1 |
| 1 | 1 | 1 | 1 | 0 |

A single linear decision boundary cannot separate XOR's positive and negative classes.

```mermaid
flowchart LR
    A[Input X1] --> C[Hidden Unit 1]
    A --> D[Hidden Unit 2]
    B[Input X2] --> C
    B --> D
    C --> E[Output Unit]
    D --> E
    E --> F[XOR Classification]

    style A fill:#2563eb,color:#fff
    style B fill:#2563eb,color:#fff
    style C fill:#0d9488,color:#fff
    style D fill:#0d9488,color:#fff
    style E fill:#7c3aed,color:#fff
    style F fill:#059669,color:#fff
```

---

## Learning Curriculum

The learning experience is divided into nine progressive modules.

| Module | Topics | Lessons |
|---|---|:---:|
| Orientation | Neural network fundamentals | 01 |
| The Single Unit | Weighted sum, activation functions, vanishing gradients | 02–06 |
| Why We Need Layers | Perceptron limitations and XOR | 07–08 |
| Feedforward Networks | Network architecture, matrix operations, softmax | 09–11 |
| Networks for NLP | Sentiment classification and pooled embeddings | 12–13 |
| Neural Language Models | N-grams, one-hot encoding, embedding lookup, inference | 14–16 |
| Training | Loss functions and gradient descent | 17 |
| Backpropagation | Forward pass, chain rule, weight updates and training | 18–22 |
| Review | Ten conceptual self-assessment questions | 23 |

---

## Learning Roadmap

```mermaid
flowchart TD
    A[Neural Network Fundamentals] --> B[Weighted Sum and Bias]
    B --> C[Activation Functions]
    C --> D[Perceptron and XOR]
    D --> E[Feedforward Networks]
    E --> F[Softmax Classification]
    F --> G[Embeddings and NLP]
    G --> H[Neural Language Models]
    H --> I[Loss and Gradient Descent]
    I --> J[Backpropagation]
    J --> K[Interactive Training]
    K --> L[Knowledge Assessment]

    style A fill:#2563eb,color:#fff
    style C fill:#0d9488,color:#fff
    style D fill:#e76f51,color:#fff
    style G fill:#7c3aed,color:#fff
    style J fill:#be185d,color:#fff
    style L fill:#059669,color:#fff
```

---

## Neural Language Model Simulation

The platform extends neural network fundamentals into Natural Language Processing.

```mermaid
flowchart LR
    A[Input Words] --> B[Embedding Lookup]
    B --> C[Embedding Concatenation]
    C --> D[Hidden Layer]
    D --> E[Output Logits]
    E --> F[Softmax]
    F --> G[Next Word Probabilities]

    style A fill:#2563eb,color:#fff
    style B fill:#0d9488,color:#fff
    style D fill:#7c3aed,color:#fff
    style F fill:#e76f51,color:#fff
    style G fill:#059669,color:#fff
```

Key concepts:

- One-hot vector representation
- Embedding matrix lookup
- Neural versus n-gram language models
- Hidden layer computation
- Probability distribution generation
- Next-word prediction
- Sentiment classification using pooled embeddings

---

## Training and Backpropagation

The training modules demonstrate how neural networks update their parameters through gradient-based optimization.

```mermaid
flowchart LR
    A[Input Data] --> B[Forward Pass]
    B --> C[Prediction]
    C --> D[Calculate Loss]
    D --> E[Backward Pass]
    E --> F[Compute Gradients]
    F --> G[Update Weights]
    G --> B

    style B fill:#2563eb,color:#fff
    style D fill:#e76f51,color:#fff
    style E fill:#7c3aed,color:#fff
    style G fill:#059669,color:#fff
```

The weight update rule:

$$
w_{\text{new}} =
w_{\text{old}}-\eta\frac{\partial L}{\partial w}
$$

Interactive implementations include:

- Forward propagation with numerical examples
- Loss calculation
- Gradient descent visualization
- Chain-rule decomposition
- Output and hidden layer weight updates
- Interactive training loop
- Training loss visualization

---

## Engineering Highlights

### Real-Time Mathematical Simulation

Neural network computations are implemented directly in JavaScript, allowing users to modify parameters and observe mathematical results immediately.

### Dynamic SVG Visualization

Network diagrams, activation curves, decision boundaries and training charts are generated using SVG.

### Lightweight Architecture

The entire application is implemented using a single HTML file containing the interface, styling, lesson content and simulation logic.

No JavaScript framework, backend server or machine learning library is required.

### Structured Learning Experience

- Categorized lesson navigation
- Session-based lesson progress tracking
- Interactive controls
- Mathematical equations
- Worked numerical examples
- Lecture slide references
- Answer-reveal review questions

---

## System Architecture

```mermaid
flowchart TD
    A[User Interaction] --> B[JavaScript Event Handlers]
    B --> C[Simulation Engine]

    C --> D[Mathematical Computation]
    C --> E[Network State]
    C --> F[Parameter Updates]

    D --> G[SVG Visualization]
    E --> G
    F --> G

    G --> H[Interactive Learning Interface]
    H --> A

    style A fill:#2563eb,color:#fff
    style C fill:#7c3aed,color:#fff
    style D fill:#0d9488,color:#fff
    style G fill:#e76f51,color:#fff
    style H fill:#059669,color:#fff
```

---

## Technology Stack

| Technology | Purpose |
|---|---|
| JavaScript | Mathematical computations and interactive simulations |
| HTML5 | Lesson structure and interface |
| CSS3 | Responsive layouts and visual styling |
| SVG | Dynamic charts and neural network diagrams |
| DOM Manipulation | Real-time interface updates |
| Google Fonts | Interface typography |
| GitHub Pages | Static website deployment |

---

## Running Locally

Clone the repository:

```bash
git clone https://github.com/arafat-rahman-lisan/neural-network-simulation.git
```

Navigate to the project directory:

```bash
cd neural-network-simulation
```

Open `index.html` in your browser.

Alternatively, start a local development server:

```bash
python -m http.server 8000
```

Visit:

```text
http://localhost:8000
```

No additional package installation or API credentials are required.

---

## Project Structure

```text
neural-network-simulation/
│
├── index.html
│
├── screencapture-arafat-rahman-lisan-github-io-neural-network-simulation-2026-11-25-01_36_14.png
├── screencapture-arafat-rahman-lisan-github-io-neural-network-simulation-2026-11-25-01_37_07.png
├── screencapture-arafat-rahman-lisan-github-io-neural-network-simulation-2026-11-25-01_37_19.png
├── screencapture-arafat-rahman-lisan-github-io-neural-network-simulation-2026-11-25-01_37_34.png
│
└── README.md
```

---

## Future Development

- Interactive CNN visualizations
- Recurrent neural network simulations
- Transformer and self-attention playground
- Interactive multi-head attention
- Persistent learning progress
- Custom dataset experimentation
- Additional mathematical exercises

These are proposed extensions to the existing platform.

---

## Developer

**Arafat Rahman**

Computer Science & Engineering

Interests: Artificial Intelligence, Machine Learning, Natural Language Processing and Interactive Learning Systems.

[GitHub Profile](https://github.com/arafat-rahman-lisan)

---

<div align="center">

## 🧠 Neural Network Lab

### Learn. Experiment. Visualize. Understand.

[Explore the Live Platform](https://arafat-rahman-lisan.github.io/neural-network-simulation/)

*Making the mathematics behind intelligent systems more accessible.*

If this project helps you understand neural networks, consider giving the repository a ⭐

</div>
