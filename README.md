# DEEPFAKE-DETECTION


# 🧠 Deepfake Detection Web Application

A deep learning-powered web application designed to detect deepfake images using a fine-tuned EfficientNet model. Built with a PyTorch backend and deployed via a Flask web server, this tool provides a simple and interactive user interface to identify whether an uploaded image is real or synthetic.

## 📌 Project Overview

Deepfakes pose a significant threat to digital authenticity. This application leverages the power of convolutional neural networks (CNNs) to accurately detect manipulated facial images. Users can upload an image, and the system returns a prediction with confidence scores.

## 🚀 Key Features

- 🖼️ Upload image via a clean web interface
- 🔍 Real-time prediction (REAL or FAKE)
- 📊 Displays model confidence score
- 💡 EfficientNet-based lightweight model
- 🧪 Trained on a curated dataset of real and fake face images

## 🧰 Tech Stack

- **Frontend:** HTML5, CSS3
- **Backend:** Python, Flask
- **Model:** PyTorch, EfficientNet
- **Utilities:** NumPy, OpenCV, PIL

## 🧠 Model Details

- **Architecture:** EfficientNet-B0
- **Training Dataset:** Deepfake/real face image dataset (custom-curated)
- **Loss Function:** CrossEntropyLoss
- **Optimizer:** Adam
- **Accuracy:** ~[Insert your test accuracy] on validation set
- **Model File:** `efficientnet_deepfake_classifier.pth`

## 📁 Directory Structure

```
deepfake-detector/
│
├── app.py                            # Flask server
├── Deepfake_model1.ipynb             # Model training notebook
├── efficientnet_deepfake_classifier.pth  # Trained model weights
├── requirements.txt                  # Dependencies
├── templates/
│   └── index.html                    # Frontend HTML (Flask compatible)
└── README.md                         # Project documentation
```

## 💻 Installation & Usage

### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/deepfake-detector.git
cd deepfake-detector
```

### 2. Create a Virtual Environment (Optional but Recommended)

```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

### 3. Install Required Packages

```bash
pip install -r requirements.txt
```

### 4. Run the Web Application

```bash
python app.py
```

Visit `http://127.0.0.1:5000/` in your browser to use the app.

## 📷 Sample Output

| Input Image | Prediction | Confidence |
|-------------|------------|------------|
| ![sample1](https://example.com/real.png) | **REAL** | 97.6% |
| ![sample2](https://example.com/fake.png) | **FAKE** | 92.3% |

## ✅ Requirements

You can generate the `requirements.txt` by running:

```bash
pip freeze > requirements.txt
```

Or use the sample content below:

```
Flask
torch
torchvision
numpy
Pillow
opencv-python
```

## 🤝 Contributing

Contributions are welcome! If you'd like to improve the model, UI, or deployment options:

1. Fork the repository
2. Create a new branch: `git checkout -b improvement-feature`
3. Commit your changes
4. Push to your branch: `git push origin improvement-feature`
5. Open a pull request


## 🙋‍♂️ Author

**Darshan**  
Data Science Undergraduate | AI Enthusiast  
