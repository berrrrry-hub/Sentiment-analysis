# 💬 Sentiment Analysis: Emotion Detection from Tweets

A class project focused on emotion classification using tweets, exploring efficient modeling strategies under computational constraints. The task involves multi-class classification with six emotion categories using transformer-based features and neural network architectures.

---

## 📌 Context
This project was completed as part of a coursework assignment in the Modern Analytics class. The dataset was sourced from a public Kaggle competition, and the goal was to accurately classify emotions in tweets (e.g., joy, sadness, love) using text-based machine learning models. The team explored various architectures while managing performance vs. efficiency trade-offs.

---

## 🎯 Objective
To build and evaluate both a simple baseline model and a more advanced multilayer perceptron (MLP) for tweet emotion classification, leveraging transformer embeddings (TinyBERT) and focusing on scalability and interpretability.

---

## 🛠 Languages & Libraries
- **Languages**: Python  
- **Libraries**: Pandas, NumPy, Matplotlib, Scikit-learn, PyTorch, Transformers (HuggingFace)

---

## 🔍 Methods Applied
- Data Cleaning and Sampling (5% and 10% subsets of the full dataset)
- Transformer-based Feature Extraction using **TinyBERT**
- Baseline Model: Single Dense Layer (for benchmarking)
- Advanced Model: **MLP** with 5 fully connected layers, ReLU, dropout, and residual connections
- Optimization: Adam with learning rate scheduling
- Loss Function: Cross-Entropy
- Evaluation Metrics: Validation Loss, Test Accuracy, Confusion Matrix

---

## 📈 Results

| Model          | Validation Loss | Test Accuracy |
|----------------|------------------|----------------|
| Baseline (1 Dense Layer) | Higher loss        | Lower accuracy |
| MLP (5 Layers, Regularized) | Lower loss        | Improved accuracy (~5–6% higher) |

- The model performed well on distinguishing **joy** and **sadness**.
- Some misclassifications occurred between **joy** and **love**, suggesting need for improved contextual understanding.

---

## ⚠️ Challenges & Solutions

| Challenge                            | Solution |
|-------------------------------------|----------|
| Large dataset and memory constraints | Used sampled subsets (5% / 10%) |
| Computational limits with transformers | Used **pre-extracted TinyBERT embeddings** |
| Overfitting in deeper models         | Applied dropout, weight decay, and early stopping |

---

## 🔑 Key Learnings
- A well-regularized MLP can capture emotional nuance effectively, even with limited data.
- Confusion matrix analysis helped identify overlapping sentiment categories needing more attention (e.g., joy vs. love).
- Trade-offs between model depth, speed, and generalization were critical in design.

---

## 🚀 Future Work
- Implement **RNN-based models** to capture sequential dependencies.
- Integrate this model into real applications like customer support chatbots or brand monitoring systems.
- Extend classification to identify harmful or abusive tweets.

---

## 👤 Contact & Portfolio
👤 **Jiaxin(Berry) Tian**  
📧 berrytian15@gmail.com  
🔗 https://github.com/berrrrry-hub?tab=repositories

