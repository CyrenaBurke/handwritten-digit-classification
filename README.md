# Handwritten Digit Classification with CNNs

This project explores how Convolutional Neural Networks (CNNs) can be used to accurately classify handwritten digits using the MNIST dataset. It was developed as part of my coursework for CPSC 585 - Artificial Neural Networks.

---

## 📌 About the Project

The ability to recognize handwritten digits has real-world applications like processing postal mail, scanning forms, and reading bank checks. In this project, I trained a CNN using TensorFlow and Keras to classify digits 0 through 9 from grayscale images.

---

## 🧠 What I Built

A custom CNN built from scratch that includes:

- Two convolutional layers
- Max pooling
- Dropout to prevent overfitting
- Dense layers for final classification

I also visualized training results and evaluated the model’s performance using a confusion matrix.

---

## 🧪 Dataset

- **MNIST dataset**: 70,000 grayscale images (28x28)
  - 60,000 used for training
  - 10,000 used for testing

Each image represents a handwritten digit (0–9). The training data was further split to include a validation set (18%).

---

## 🔧 Model Architecture

Here’s a breakdown of the layers:

- `Conv2D(16 filters, 5x5) + ReLU`
- `MaxPooling2D(2x2)`
- `Dropout(0.3)`
- `Conv2D(32 filters, 3x3) + ReLU`
- `MaxPooling2D(2x2)`
- `Dropout(0.3)`
- `Flatten → Dense(100, ReLU)`
- `Dropout(0.4)`
- `Dense(10, softmax)`

---

## ✅ Results

- **Test Accuracy:** 98.9%
- Very strong performance across all digit classes
- Most confusion occurred between digits like 4 and 9
- Training was efficient and showed minimal overfitting

---

## 📊 Visualizations

- `accuracy.png`: Training vs validation accuracy over 12 epochs
- `confusionmatrix.png`: Heatmap of model predictions vs true labels
- `numbers.png`: Sample images from the dataset

---

## 🚀 How to Run This

1. **Clone the repo:**

```bash
git clone https://github.com/CyrenaBurke/handwritten-digit-classification.git
cd handwritten-digit-classification
```

2. **Set up a virtual environment:**

```bash
python -m venv venv
source venv/bin/activate        # Windows: venv\Scripts\activate
```

3. **Install required packages:**

```bash
pip install -r requirements.txt
```

4. **Run the script:**

```bash
python mnist_cnn_project.py
```

---

## 📁 Project Files

- `mnist_cnn_project.py` — CNN training + evaluation
- `Final_Report.docx` — MLA-formatted project report
- `MNIST_CNN_Presentation.pptx` — Slides for presentation
- `requirements.txt` — All required Python packages

---

## 🙋‍♀️ Author

**Cyrena Burke**  
CPSC 585 – Artificial Neural Networks  
California State University, Fullerton

---

## 📚 References

- LeCun, Y., Bottou, L., Bengio, Y., & Haffner, P. (1998). Gradient-based learning applied to document recognition.
- TensorFlow and Keras Documentation
- [MNIST Dataset](http://yann.lecun.com/exdb/mnist/)
