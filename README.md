# DL_Image_Text_Classification

## 📌 Project Summary  
This project explored **two applications of deep learning**:  
1. 🚗 **Accident Severity Prediction from Images**  
2. 💬 **Sentiment Analysis of Spanish Tweets**  

The aim was to experiment with multiple architectures, improve performance, and apply interpretability techniques for better model understanding.  

---

## 🚗 Part 1: Accident Severity Prediction  
- **Goal:** Predict road accident severity from images to support emergency response, insurers, and transport authorities.  
- **Models Tested:**  
  - 🔹 Multi-Layer Perceptrons (MLPs) → Best accuracy **66%** with dropout & batch normalization.  
  - 🔹 CNN (baseline) → Accuracy improved with **data augmentation**.  
  - 🔹 Transfer Learning:  
    - VGG16 → **61% accuracy**  
    - ResNet50 → **72% accuracy** (best performer)  
- **Interpretability:** Layer activations & maximally activating images to visualize what the CNN focused on.  
- **Conclusion:** **ResNet50** delivered the highest performance for accident classification.  

---

## 💬 Part 2: Sentiment Analysis of Tweets  
- **Goal:** Classify Spanish tweets into **positive** or **negative** sentiment.  
- **Dataset:** Tweets originally labeled with 6 emotions, regrouped into binary sentiment.  
- **Models Tested:**  
  - 🔹 RNN-LSTM → **73% accuracy**, but overfitting issues.  
  - 🔹 RNN-GRU → **69% accuracy**, less effective.  
  - 🔹 CNN for Sequential Data → **91% accuracy** (best performer).  
- **Attention Mechanism:** Highlighted important words influencing predictions.  
- **Conclusion:** CNN generalized better on small datasets, outperforming RNNs.  

---

## 🏆 Overall Conclusion  
- 🚗 **Images:** ResNet50 (transfer learning) achieved the best accuracy (**72%**).  
- 💬 **Text:** CNN outperformed LSTM/GRU with **91% accuracy**.  
- 🔑 The project highlights the trade-offs between **model complexity, accuracy, and interpretability** in deep learning across different data modalities.  
