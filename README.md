# 💼 Portfolio Guide

Welcome to my portafolio! Here you'll discover a collection of projects I've worked on, including my personal insights, conclusions, and lessons learned.

## Index
- [🎲 Probability and Decision Analysis](#-probability-and-decision-analysis)
- [🤖 Machine Learning](#-machine-learning)
- [🚀 Optimization and Operations Research](#-optimization-and-operations-research)
- [⭐ Recommender Systems](#-recommender-systems)
- [🧠 Deep Learning](#-deep-learning)
- [🧑‍💻 Generative & Agentic AI](#-generative--agentic-ai)
- [📊 AI Strategy & Governance](#-ai-strategy--governance)

## 🎲 Probability and Decision Analysis

| Repository | Description | Decision focus |
| --- | --- | --- |
| [Physician Schedule Optimization](https://github.com/techbysaels/physician-schedule-optimization/blob/62673bc2e6a1cc532df6765e2715df9b5107935e/README.md) | Uses a binomial attendance model to compare appointment-booking levels when patients may not attend and a physician has limited daily capacity. | Balances unused capacity against overbooking risk. Shows why expected attendance alone is insufficient for setting a booking policy. |
| [Warehouse Fulfillment Probability](https://github.com/techbysaels/warehouse-fulfillment-probability/blob/f57e6939c6836851370c6fb0d081a588bd636dff/README.md) | Models aggregate demand across stores with Normal distributions and calculates service probabilities and inventory requirements. Includes a memorandum translating the analysis into an inventory recommendation. | Explains risk pooling and the supply-service trade-off, with particular attention to the assumption that store demands are independent. |

## 🤖 Machine Learning

| Repository | Description | Methods and review focus |
| --- | --- | --- |
| [Airline Customer Segmentation](https://github.com/techbysaels/airline-customer-segmentation/blob/0d501bd679cc3021c6e1c04e534e9e6b4e703c6b/README.md) | Explores loyalty segments using account age and mileage balance. | K-Means and cluster interpretation on a small illustrative sample. Documents the need for feature scaling, more observations, and campaign validation. |
| [Mall Customer Segmentation](https://github.com/techbysaels/mall-customer-segmentation/blob/231f16bfa6816a8bdbbcef8ca864e5b036f81c84/README.md) | Groups customers by age, income, and spending score to develop differentiated marketing hypotheses. | Standardization, elbow-based cluster selection, K-Means, and segment profiling. Connects the groups to potential loyalty and re-engagement strategies. |
| [Automobile Customer Segmentation](https://github.com/techbysaels/automobile-customer-segmentation/blob/9e6f9573031101fdd15d583619bf40ce9bcbafb6/README.md) | Explores customer preferences using binary survey attributes and identifies potential segments for research and marketing. | Correlation analysis, hierarchical views, K-Means, and PCA visualization. Discusses stability checks and methods better suited to binary similarity. |
| [Bike Rental Demand Prediction](https://github.com/techbysaels/bike-rental-demand-prediction/blob/869552e5aa239391e4337496f424acfa5cc5504f/README.md) | Predicts rental demand from weather and calendar variables to support capacity planning. | Compares linear regression with regression trees and cost-complexity pruning. Examines overfitting and the trade-off between predictive performance and interpretability. |
| [Loan Default Prediction](https://github.com/techbysaels/loan-default-prediction/blob/914f87c6378f9bd9aac7140e0369f58c717472d4/README.md) | Compares default-risk models using both classification performance and a simplified lending-profit framework. | Logistic regression, decision trees, XGBoost, and threshold analysis. Connects model selection to the different costs of approving defaulters and declining reliable borrowers. |
| [Diabetes Prediction](https://github.com/techbysaels/diabetes-prediction/blob/a74dc324095f3ecb0992888f33e050e0c336c5f9/README.md) | Contains two distinct studies: continuous disease-progression estimation and binary diabetes-risk classification. | Ordinary least squares and feature reduction for progression; XGBoost for risk classification. Keeps the prediction targets and their evaluation metrics separate. |
| [Breast Cancer XGBoost Classifier](https://github.com/techbysaels/breast-cancer-XGBoost-classifier/blob/63e35bf6201e36fa21b23a777b0900cdbde98ca0/README.md) | Classifies benign and malignant samples using structured features derived from digitized images. | XGBoost, held-out evaluation, and feature importance. Identifies sensitivity, calibration, and external validation as necessary follow-up work before clinical use. |

## 🚀 Optimization and Operations Research

| Repository | Description | Methods and decision focus |
| --- | --- | --- |
| [Retail Pricing Optimization](https://github.com/techbysaels/retail-pricing-optimization/blob/c01ab1bee72afa4b78c1a75be8b1f96ed4f8e14d/README.md) | Optimizes weekly revenue using a demand equation with current prices, lagged prices, and seasonal effects. | Four Gurobi formulations progress from continuous prices to discrete price ladders and promotion restrictions, making recommendations consistent with merchandising rules. |
| [Landfill Network Optimization](https://github.com/techbysaels/landfill-network-optimization/blob/7e584c4ff4205cec182d12464558963606a24c8f/README.md) | Minimizes transportation cost across generation centers, transfer depots, and landfills, including network-expansion scenarios. | A Gurobi network-flow model enforces supply, capacity, flow-conservation, and demand constraints. The analysis connects the resulting shipment plan to cost and capacity assumptions. |

## ⭐ Recommender Systems

| Repository | Description | Methods and evaluation focus |
| --- | --- | --- |
| [Movie Rating Collaborative Filtering](https://github.com/techbysaels/movie-rating-collaborative-filtering/blob/c4270c23d0c14a5aba06bc26db2fd24afd7f9ff8/README.md) | Estimates missing MovieLens ratings from shared user-movie preference patterns. | Sparse matrices, validation masking, and SoftImpute compared with an average-rating baseline. The training-validation gap motivates closer attention to generalization. |
| [Music Rating Collaborative Filtering](https://github.com/techbysaels/music-rating-collaborative-filtering/blob/25f7cfe48c0cadc48b48568522fab2004554b464/README.md) | Predicts listener preferences from incomplete user-song ratings. | Low-rank matrix completion and held-out rating evaluation. Discusses ranking metrics, diversity, catalog coverage, and cold-start handling as next steps. |
| [Jester Joke Rating Collaborative Filtering](https://github.com/techbysaels/jester-joke-rating-collaborative-filtering/blob/1e777e1e7b57796745b8810e4d0a099184ba42dc/README.md) | Applies collaborative filtering to subjective humor preferences. | SoftImpute and in-sample versus out-of-sample evaluation. Provides another setting for examining rating reconstruction and the limits of using it alone to evaluate a recommender. |

## 🧠 Deep Learning

| Repository | Description | Methods and review focus |
| --- | --- | --- |
| [Heart Disease Prediction](https://github.com/techbysaels/heart-disease-prediction/blob/cecb41325057214513a4cedb4cd864b7119d6d74/README.md) | Contains separate neural-network studies of structured clinical features and normal versus abnormal ECG5000 traces. | Compares the engineering requirements of tabular and waveform inputs. The two datasets address different tasks, so their accuracy scores are not a direct model comparison. |
| [IMDb Review Sentiment Classification](https://github.com/techbysaels/movie-sentiment-classification/blob/3b30bfe7f6509fc2b9ae369685be21284510ded4/README.md) | Classifies movie reviews as positive or negative to illustrate scalable feedback triage. | Multi-hot text vectorization and a feed-forward neural network. Establishes a compact NLP baseline while documenting the loss of word order and context. |
| [Clothes Classifier](https://github.com/techbysaels/clothes-classifier/blob/605a4dc1bc11bda50afd128d06ecd0de4b376d10/README.md) | Classifies Fashion-MNIST images into ten clothing categories. | Compares a fully connected network with a CNN on the same dataset to examine the value of preserving spatial structure. |
| [Handbags vs. Shoes Classifier](https://github.com/techbysaels/handbag-shoes-classifier/blob/816607d9522781704fb2c84ca2b7b69b43aa990b/README.md) | Explores product-image classification with fewer than 100 training images. | Compares a baseline CNN, data augmentation, and ResNet50 transfer learning. Interprets results in light of the small test set. |
| [Sign Language Classifier](https://github.com/techbysaels/sign-language-classifier/blob/0a0b863705762ef28385a10318f69b5c153bea8b/README.md) | Recognizes 24 static ASL letter classes from grayscale hand images. | CNN training and image preprocessing. Records invalid-value and validation-loss issues that need investigation; the task does not cover full sign-language translation. |

## 🚀 Generative & Agentic AI

| Repository | Description | Implementation focus |
| --- | --- | --- |
| [Nexqori — Language and Voice](https://github.com/nexqori/factored-hackathon-2026-nexqori/blob/2abf585bec4e48ac2f02148509c0be4be372f978/README.md) | A conversational banking prototype that helps customers investigate charges, prepare complaints, and follow their resolution. An administrator reviews the evidence and authorizes refunds. Combines Jev intent and safety classification with a conversation and workflow engine to investigate transactions, prepare complaints, and retrieve resolution status. Uses OpenAI capabilities to support a banking conversation in Spanish, English, and Portuguese, with optional live voice. | React and TypeScript, FastAPI, PostgreSQL, text and optional voice interaction, document generation, and configurable notifications. Ownership checks, confirmation, and idempotency govern actions. Customer confirmation, ownership checks, idempotency, and administrator approval define what the assistant may do. Status queries report existing outcomes rather than issuing another refund. Connects natural-language interaction to transaction and complaint context. The backend remains responsible for authenticated actions and stored workflow state. |

## 📊 AI Strategy & Governance

| Repository | Description | Practical contribution |
| --- | --- | --- |
| [Fairness and Bias](https://github.com/techbysaels/fairness-and-bias/blob/7008bdcd3c280f0c1a527abf0429ccf1e89f9548/README.md) | Studies lending fairness, a repayment-model audit, facial-recognition failure, protected attributes, and representation versus measurement bias. | Connects subgroup metrics and threshold trade-offs to data quality, review procedures, and governance. Demonstrates why removing a protected attribute does not by itself establish fairness. |
| [Interpretability and Causality](https://github.com/techbysaels/interpretability-and-causality/blob/db1edabff0662473bff9cc4d7c7043d8439c6b0c/README.md) | Examines insurance telematics, medical AI, high-impact decision systems, and Integrated Gradients for image classification. | Separates explaining a prediction from establishing the effect of an intervention. Uses attribution as a diagnostic tool while making its limits explicit. |
| [Data, Models, and Decisions](https://github.com/techbysaels/data-models-and-decisions/blob/ac7b11d3ff580f0a4029d6cb7a837fd8437193a9/README.md) | Analyzes use cases across supply chains, checkout-free retail, fleet safety, cinema operations, agriculture, infrastructure, software, accounting, and restaurants. | Matches process needs to rules, machine learning, sensing, optimization, and human review. Makes data requirements and decision ownership part of the system design. |
| [Leading Digital Transformations](https://github.com/techbysaels/leading-digital-transformations/blob/06e337727ca9b6be142235aaa8281d8ac4a0fe6f/README.md) | Brings together NASA open innovation, the Littoral Combat Ship program, business translators, a fleet-monitoring transformation, and an IoT-company transformation playbook. | Examines adoption, interdependent delivery risks, shared priorities, pilots, and measurable outcomes. |
