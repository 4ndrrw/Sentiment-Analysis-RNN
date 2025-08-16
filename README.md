# ​ Sentiment Analysis RNN

![Sentiment RNN Banner](sentiment.png)

**A Recurrent Neural Network (RNN)-based model for sentiment classification of texts (e.g., movie reviews, tweets).**  
*Processes sequential text data using word embeddings and an LSTM or SimpleRNN layer for binary sentiment prediction.*

---

## ​ Features

- 💬 **Text Preprocessing**: Tokenization, padding/truncating sequences to a fixed length.  
- 🆔 **Embedding Layer**: Converts words into dense vector representations.  
- 🔁 **RNN Architecture**: Utilizes SimpleRNN or LSTM for capturing temporal dependencies.  
- 🎯 **Binary Classification**: Outputs sentiment labels (positive vs. negative) via sigmoid activation.  
- 🏆 **Training & Evaluation**: Includes training with train/validation/test split and evaluation metrics (accuracy, loss).

---

## ​ Dataset

- **Sample Dataset**: Could be IMDb reviews or a custom dataset (e.g., tweets, product reviews).  
- **Preprocessing Steps**:
  - Text cleaning (lowercasing, removing punctuation)
  - Tokenization
  - Converting words to sequences
  - Padding to a standardized maximum length

---

## ​ Model Architecture

**RNN-based architecture** consisting of:

1. **Embedding Layer** (e.g., `Embedding(input_dim, output_dim, input_length=max_len)`)  
2. **Recurrent Layer**: SimpleRNN or LSTM with a specified number of units  
3. **Dense Output Layer** with `sigmoid` activation for binary sentiment output  
4. **Loss Function**: Binary Cross-Entropy  
5. **Optimizer**: Adam (or any gradient-based optimizer)

---

## ​​ Installation

```bash
# Clone the repository
git clone https://github.com/4ndrrw/Sentiment-Analysis-RNN.git
cd Sentiment-Analysis-RNN

# Create virtual environment
python -m venv venv
source venv/bin/activate  # Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt
```

---

## 📊 Results

- **Mean Absolute Error (MAE)**:  8.15%
- **Mean Squared Error (MSE)**:   1.56%
- **R-squared (R² Score)**:       0.7874
- **Loss Curve**:  
  ![Training Loss](final_model_loss.png)  
- **Predicted vs. Actual Scores**:  
  ![Scatterplot](final_model_scatterplot.png)  

---

## ⚙️ Tech Stack

![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?logo=tensorflow&logoColor=white)
![Keras](https://img.shields.io/badge/Keras-D00000?logo=keras&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?logo=numpy&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?logo=pandas&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557C?logo=matplotlib&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?logo=jupyter&logoColor=white)
![VS Code](https://img.shields.io/badge/VS%20Code-0078D4?logo=Visual%20Studio%20Code&logoColor=white)

---

## 🤝 Contributing

1. Fork the repository.  
2. Create a new branch (`git checkout -b feature-branch`).  
3. Commit your changes (`git commit -am 'Add new feature'`).  
4. Push to the branch (`git push origin feature-branch`).  
5. Open a Pull Request.

---
