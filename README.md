# News-Topic-Classifier-Using-BERT

A deep learning based **News Topic Classification Web App** built using **BERT**, **Hugging Face Transformers**, and **Streamlit**.

This project fine-tunes the `bert-base-uncased` model on the AG News dataset to classify news headlines into four categories:

- 🌍 World
- ⚽ Sports
- 💼 Business
- 🔬 Sci/Tech

The trained model is deployed as an interactive Streamlit web application and exposed publicly using Ngrok.

---

##  Features

✅ Fine-tuned BERT model using Hugging Face Transformers  
✅ Real-time news headline classification  
✅ Confidence score visualization  
✅ Streamlit interactive web interface  
✅ Balanced dataset training for better performance  
✅ Public deployment using Ngrok  

---

##  Technologies Used

- Python
- PyTorch
- Hugging Face Transformers
- Hugging Face Datasets
- Scikit-learn
- Streamlit
- Ngrok

---

##  Dataset

This project uses the AG News dataset from Hugging Face.

Dataset contains 4 categories:

| Label | Category |
|------|-----------|
| 0 | World |
| 1 | Sports |
| 2 | Business |
| 3 | Sci/Tech |

---

##  Model Details

### Pretrained Model
`bert-base-uncased`

### Training Configuration

- Epochs: 3
- Learning Rate: 2e-5
- Batch Size: 16
- Weight Decay: 0.01
- Warmup Ratio: 0.1

### Evaluation Metrics

- Accuracy Score
- Weighted F1 Score

---

##  Training Strategy

To make training faster and balanced, the dataset was sampled equally:

- 2500 samples per class
- Total training samples = 10,000

This helps reduce class imbalance and improves model fairness.

---

##  Streamlit App

The Streamlit interface allows users to:

- Enter a news headline
- Predict the news category
- View confidence scores for all classes

Example:

Input:
Tesla stock surges after record earnings

Prediction:
💼 Business — 98.2% confidence

---

##  Installation

Clone the repository:

```bash
git clone https://github.com/your-username/bert-news-classifier.git
cd bert-news-classifier

👨‍💻 Author

Developed by [Yahya Abbasi]
