# 🐶 Dog Breed Classification using Transfer Learning (TensorFlow, Colab)

This project classifies dog images into different breeds using deep learning and transfer learning techniques. The model is trained using TensorFlow and EfficientNetB0 architecture. Built and executed fully on Google Colab.

---

## 📁 Dataset
- Source: [Kaggle Dog Breed Identification](https://www.kaggle.com/c/dog-breed-identification/data)
- Number of classes: 120
- Format: Images in `.jpg`, with labels provided in a `.csv` file

---

## 🧠 Model Architecture
- Base Model: `EfficientNetB0` (pretrained on ImageNet)
- Top Layers:
  - Global Average Pooling
  - Dropout
  - Dense Layer (Softmax activation)

**Training Setup:**
- Optimizer: Adam
- Loss: Categorical Crossentropy
- Epochs: 5–10 (depending on GPU time)
- Image size: 224x224
- Data Augmentation applied via `ImageDataGenerator`

---

## 📊 Results

| Metric              | Value (approx) |
|---------------------|----------------|
| Training Accuracy   | ~95%           |
| Validation Accuracy | ~89%           |
| Test Accuracy       | ~88%           |

*(Exact numbers depend on runtime conditions and data split)*

---
## 🚀 How to Run
1. Clone this repository
2. Open the notebook in [Google Colab](https://colab.research.google.com/)
3. Upload your Kaggle API key (`kaggle.json`)
4. Run all cells

---

## 🛠️ Tech Stack
- Python 3.x
- TensorFlow / Keras
- EfficientNetB0
- Google Colab
- Matplotlib / NumPy / Pandas

---

## 📌 Future Work
- Improve performance with longer training or deeper models
- Add confusion matrix and class-wise metrics
- Deploy via Streamlit or Gradio
- Convert to TensorFlow Lite for mobile use

---

## 🙌 Acknowledgements
Inspired by [Daniel Bourke's Dog Vision Project](https://github.com/mrdbourke/zero-to-mastery-ml).

---

**Author:** [Your Name]  
**GitHub:** [@yourusername](https://github.com/yourusername)

