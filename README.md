# 🐛 Pest Analysis using Convolutional Neural Networks (CNN)

This project aims to detect and classify pests — specifically **Fall Armyworm** — using a trained Convolutional Neural Network (CNN) model. The model is built and trained using image data to help automate pest detection for agricultural support.

## 📌 Project Overview

- **Goal**: Early detection of crop pests to assist in timely intervention.
- **Target Pest**: Fall Armyworm (_Spodoptera frugiperda_)
- **Model Type**: CNN (.h5 Keras model)
- **Dataset**: Custom image dataset of pests (classified as infected/uninfected or multiple pest types).
- **Framework**: TensorFlow / Keras

## 🧠 Model

The trained model file is:
```
fall_armyworm_cnn.h5
```

> **Note:** Due to the file size, this is tracked using [Git Large File Storage (LFS)](https://git-lfs.github.com/).

## 📂 Project Structure

```
Pest-Analysis/
├── fall_armyworm_cnn.h5       # Trained CNN model
├── images/                    # Sample/test images
├── notebooks/                 # Jupyter Notebooks for training/testing
├── src/                       # Source code for data loading, training, etc.
├── requirements.txt           # Project dependencies
└── README.md                  # Project description
```

## 🚀 How to Run

1. **Clone the repository**
   ```bash
   git clone https://github.com/Salrahim21/Pest-Analysis.git
   cd Pest-Analysis
   ```

2. **(Optional) Create a virtual environment**
   ```bash
   python -m venv env
   source env/bin/activate  # On Windows: env\Scripts\activate
   ```

3. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

4. **Run inference**
   You can load the model in a script or Jupyter Notebook:
   ```python
   from tensorflow.keras.models import load_model
   model = load_model("fall_armyworm_cnn.h5")
   ```

5. **Make predictions**
   Pass an image through preprocessing and use `model.predict()`.

## 🛠️ Technologies Used

- Python
- TensorFlow / Keras
- NumPy, OpenCV, Matplotlib
- Git & GitHub
- Git LFS (for large model files)

## 📈 Future Work

- Expand dataset to include more pest species
- Deploy model via a Flask API or web interface
- Integrate with mobile apps for real-time pest detection

## 📄 License

This project is open-source and available under the [MIT License](LICENSE).

## 👨‍💻 Author

**Salrahim21**  
GitHub: [@Salrahim21](https://github.com/Salrahim21)
