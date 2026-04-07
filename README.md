# Multimodal AI for Heart Failure Risk Stratification
This project presents a multimodal machine learning framework for risk stratification in patients with heart failure, integrating heterogeneous clinical and diagnostic data.

## Project Overview
Heart failure is a major cause of hospitalization and mortality worldwide. Accurate risk stratification is crucial to identify patients at high risk of adverse events and support clinical decision-making.
This project proposes a multimodal system that combines:
- Electronic Health Records (EHR)
- Electrocardiogram (ECG) signals
- Echocardiography data
The goal is to classify patients into low, medium, and high-risk categories based on their probability of adverse outcomes.

## Methodology
A dedicated architecture is designed for each data modality:
- **EHR data**: processed using feature selection (RFE) and modeled with XGBoost
- **ECG signals**: analyzed using a 1D ResNet with Squeeze-and-Excitation blocks
- **Echocardiography**: processed with a 3D Convolutional Neural Network
The outputs of each model are combined using a **decision-level fusion (soft voting)** strategy to obtain the final prediction.

## System Overview
The following diagram illustrates the proposed multimodal framework:
![Multimodal Pipeline](pipeline.png)

## Key Features
- Multimodal data integration (clinical + signal + imaging)
- Combination of machine learning and deep learning models
- Decision-level fusion for robust prediction
- Explainability techniques (SHAP, Grad-CAM, Integrated Gradients)
- Uncertainty estimation based on inter-modality agreement

## Clinical Relevance
The system is designed as a clinical decision support tool to:
- Improve early identification of high-risk patients
- Support hospitalization and discharge decisions
- Reduce unnecessary hospitalizations
- Enable personalized patient management

## Project Type
This is a research-oriented project focused on system design and methodology development.

## Report
The full project report is available here:
[Project Report](Multimodal%20Approach%20for%20Heart%20Failure%20Risk%20Stratification.pdf)
