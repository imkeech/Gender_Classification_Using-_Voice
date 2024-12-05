# 🎤 Gender Recognition from Audio Data

This project focuses on **gender recognition** using audio features extracted from speech recordings. The model predicts the gender of a speaker based on the audio input, leveraging advanced machine learning techniques.

---

## ✨ Features

- **Audio Preprocessing**: Converts raw audio into feature-rich data for analysis.
- **Machine Learning Models**:
  - Sequential LSTM/GRU Models for sequence analysis.
  - SVM and Random Forest classifiers for efficient predictions.
- **Performance Metrics**: Includes accuracy and F1-score for robust evaluation.

---

## 📂 Project Structure

- `load_audio_files_with_lengths()`: Preprocesses audio files, extracting data and lengths.
- **Models**:
  - Deep learning using TensorFlow.
  - Classical machine learning with Scikit-learn.
- **Evaluation**:
  - Metrics like accuracy and F1-score are calculated for model comparison.
- **Visualization**:
  - Model performance is visualized using Matplotlib.

---

## 🛠️ Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/your-repo-name/gender-recognition.git
   cd gender-recognition
   ```
2. Install the required Python libraries:
   ```bash
   pip install -r requirements.txt
   ```

---

## 🚀 How It Works

1. **Data Loading**:
   - The `librosa` library processes `.flac` files to extract raw audio and duration.

   ```python
   audio, sr = librosa.load(file_path, sr=None)
   ```

2. **Feature Extraction**:
   - Mel-frequency cepstral coefficients (MFCC) are extracted for better speech analysis.

3. **Modeling**:
   - Recurrent Neural Networks (LSTM/GRU) handle time-series data.
   - Support Vector Machines (SVM) and Random Forests for quick classification.

4. **Evaluation**:
   - Compare models using:
     ```python
     accuracy = accuracy_score(y_true, y_pred)
     f1 = f1_score(y_true, y_pred, average="weighted")
     ```

---



![Model Workflow](https://media.giphy.com/media/26AHONQ79FdWZhAI0/giphy.gif)
### 📊 Metrics Visualization

Include performance graphs like the one below to make your README more engaging:

```python
plt.plot(history.history['accuracy'], label='Train Accuracy')
plt.plot(history.history['val_accuracy'], label='Validation Accuracy')
plt.legend()
plt.show()
```

---

## 📈 Results

- **Best Model**: LSTM achieved an F1-score of 92%.
- **Insights**:
  - Audio length significantly impacts prediction accuracy.
  - Proper preprocessing is crucial for robust gender recognition.

---

## 🤝 Contributing

1. Fork the repository.
2. Create a feature branch:
   ```bash
   git checkout -b feature-name
   ```
3. Submit a Pull Request.

---

## 📧 Contact

For any inquiries, feel free to reach out:
- Email: krishnavkn22@example.com
- GitHub: https://github.com/imkeech

---
