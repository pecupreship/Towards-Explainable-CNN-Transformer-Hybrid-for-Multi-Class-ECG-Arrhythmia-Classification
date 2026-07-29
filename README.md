**Towards Explainable CNN-Transformer Hybrid for Multi-Class ECG Arrhythmia Classification**
Overview

This project presents Attention-Based explainable CNN-Transformer hybrid deep learning framework for automated multi-class ECG arrhythmia classification using the MIT-BIH Arrhythmia Dataset. The architecture combines Convolutional Neural Networks (CNNs) for local ECG waveform feature extraction with Transformer encoders for long-range temporal dependency learning.

In addition to predictive modeling, the framework incorporates attention-based explainability to improve interpretability, transparency, and trustworthiness in healthcare AI systems.

**Research Motivation**

Electrocardiography (ECG) remains one of the most important non-invasive tools for diagnosing cardiovascular abnormalities. However, manual ECG interpretation can be time-consuming and highly dependent on clinical expertise.

Recent advances in deep learning and Transformer architectures have demonstrated strong capabilities in sequential data modeling. This project investigates the application of a CNN-Transformer hybrid framework for ECG arrhythmia classification while integrating explainable AI mechanisms for interpretable clinical decision support.

## Objectives

- Develop a CNN-Transformer hybrid ECG classification framework
- Perform automated multi-class arrhythmia classification
- Learn local ECG morphology and long-range temporal dependencies
- Evaluate model performance using clinically relevant metrics
- Incorporate attention-based explainable AI for interpretable predictions

## Dataset
MIT-BIH Arrhythmia Database

The project utilizes the publicly available MIT-BIH Arrhythmia Database from PhysioNet.

## Selected Heartbeat Classes

| Label | ECG Symbol | Description |
|---|---|---|
| 0 | N | Normal Beat |
| 1 | V | Premature Ventricular Contraction (PVC) |
| 2 | A | Atrial Premature Beat (APB) |

---

## ECG Signal Preprocessing

The preprocessing pipeline included:

- heartbeat-centered ECG segmentation
- fixed-length signal extraction
- signal normalization
- label encoding
- train-test splitting

Heartbeat-centered segmentation preserved clinically meaningful waveform morphology for deep learning-based ECG sequence analysis.

## CNN-Transformer Hybrid Architecture

To improve local waveform representation and computational efficiency, the baseline Transformer architecture was extended into a CNN-Transformer hybrid framework. The convolutional layers extracted local ECG morphology features such as QRS complexes and waveform patterns, while the Transformer encoder modeled long-range temporal dependencies for multi-class arrhythmia classification.

Architecture Pipeline
ECG Signal
     ↓
1D CNN Layers
     ↓
Local ECG Features
     ↓
Transformer Encoder
     ↓
Global Mean Pooling
     ↓
Fully Connected Layer
     ↓
Multi-Class Prediction
Self-Attention Mechanism

The Transformer encoder relies on self-attention mechanisms to capture contextual relationships between ECG sequence positions.

**Explainable AI (XAI)**

Attention-based explainability was incorporated to visualize diagnostically important ECG regions contributing to classification decisions. The generated attention maps provided interpretable insights into temporal ECG dependencies learned by the Transformer encoder.

This supports:

- interpretable healthcare AI
- trustworthy prediction systems
- clinically meaningful model analysis

---

## Evaluation and Research Insights

The model was evaluated using clinically relevant metrics including:

- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix

Because medical datasets are frequently class-imbalanced, overall accuracy alone was insufficient for reliable clinical evaluation. Confusion matrix analysis enabled detailed class-wise assessment of arrhythmia detection performance and revealed clinically important misclassification patterns across heartbeat categories.

The model also exhibited reduced sensitivity toward minority arrhythmia classes, highlighting the practical impact of class imbalance in ECG classification tasks. These observations reflect real-world challenges commonly encountered in healthcare AI and medical time-series classification research.

## Technologies Used

| Technology | Purpose |
|---|---|
| Python | Core programming language |
| PyTorch | Deep learning framework |
| NumPy | Numerical computing |
| Matplotlib | Visualization |
| Scikit-learn | Evaluation metrics |
| WFDB | ECG signal processing |
| Google Colab | Model training environment |

---

## Key Features

- CNN-Transformer hybrid architecture
- Multi-class arrhythmia classification
- Attention-based temporal learning
- Attention-Based Explainable AI integration
- Confusion matrix analysis
- GPU-compatible training workflow
- Research-oriented implementation


**Research Significance**

This project demonstrates the application of CNN-Transformer hybrid architectures in healthcare time-series analysis and contributes toward the development of interpretable and explainable AI systems for automated cardiac diagnosis.


**Results and Findings**

The CNN-Transformer hybrid architecture demonstrated effective ECG feature learning by combining convolutional feature extraction with Transformer-based temporal modeling. The convolutional layers improved local waveform representation, while the Transformer encoder captured global contextual dependencies across ECG sequences.

The project also highlighted practical research challenges including:

- class imbalance handling
- minority class sensitivity analysis

**Author**

Ekundayo Olorunfemi Matthew
## Research Interests

- Medical Artificial Intelligence
- Explainable AI (XAI)
- Transformer Architectures
- Healthcare Data Science
- Deep Learning

