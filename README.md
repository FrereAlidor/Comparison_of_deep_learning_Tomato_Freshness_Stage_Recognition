# Comparison_of_deep_learning_Tomato_Freshness_Stage_Recognition

Here's a complete `README.md` file in **English** for your GitHub project **"Comparison of Deep Learning Models for Tomato Freshness Stage Recognition"**. It includes a clear overview, setup instructions, results table, and a note about the mobile app demo.

---

```markdown
# 🍅 Comparison of Deep Learning Models for Tomato Freshness Stage Recognition

This project presents a comparative study of three deep learning models — **YOLOv5m**, **Xception**, and a **Vision Transformer** — for the classification of tomato freshness stages: **Fresh**, **At-risk**, and **Rotten**. The project also includes a mobile application demo for real-time prediction.

## 📽️ Mobile App Demo

You can find a video demonstration of the mobile app under the [`Application_detector/`](./Application_detector) folder.

> ⚠️ Note: The APK file exceeds GitHub’s recommended file size. You may consider using [Git LFS](https://git-lfs.github.com) for better handling of large files.

---

## 📊 Dataset

The dataset used for this project consists of images categorized into three classes:

- `Fresh`
- `At-risk`
- `Rotten`

All images were preprocessed and augmented to ensure robustness and generalization across different lighting and environmental conditions.

---

## 🚀 Models Trained

We trained and evaluated the following models:

- **YOLOv5m**: Object detection and classification
- **Xception**: Convolutional neural network architecture
- **Vision Transformer (ViT)**: Transformer-based image classification

---

## 🧪 Performance Comparison

| **Model**     | **Metric**   | **At-risk (%)** | **Fresh (%)** | **Rotten (%)** | **Overall Accuracy (%)** | **Training Time** | **Prediction Time / image** |
|--------------|--------------|------------------|----------------|----------------|----------------------------|--------------------|-----------------------------|
| YOLOv5m       | Accuracy     | 98.33            | 100.00         | 100.00         | **99.44**                  | 2:33:57            | 156.1 ms                    |
|              | Precision    | 98.33            | 100.00         | 100.00         |                            |                    |                             |
|              | Recall       | 98.33            | 100.00         | 100.00         |                            |                    |                             |
|              | F1-score     | 99.15            | 100.00         | 99.17          |                            |                    |                             |
| Xception      | Accuracy     | 99.00            | 98.25          | 98.72          | 98.67                      | 1:46:01            | 762.0 ms                    |
|              | Precision    | 97.70            | 98.60          | 99.68          |                            |                    |                             |
|              | Recall       | 99.00            | 98.25          | 98.72          |                            |                    |                             |
|              | F1-score     | 98.35            | 98.42          | 99.20          |                            |                    |                             |
| Transformer   | Accuracy     | 100.00           | 99.00          | 99.00          | **99.56**                  | 4:40:35            | 33.9 ms                     |
|              | Precision    | 99.12            | 99.72          | 99.67          |                            |                    |                             |
|              | Recall       | 98.83            | 99.48          | 99.39          |                            |                    |                             |
|              | F1-score     | 98.97            | 99.60          | 99.53          |                            |                    |                             |

---

## 📱 Application

A mobile application was developed using the YOLOv5m model to demonstrate real-world usage. It allows for the detection and classification of tomato freshness stages using a smartphone camera.

---

## 📁 Repository Structure

```

.
├── Application\_detector/        # Contains the APK and mobile code
├── Data/                        # Dataset used for training and validation
├── Model\_YOLOv5m/               # YOLOv5m model training and scripts
├── Model\_Xception/              # Xception model training scripts
├── Model\_Transformer/           # Vision Transformer training scripts
├── results/                     # Evaluation results and plots
├── README.md                    # Project documentation
└── ...

````

---

## 🛠️ Installation & Usage

1. **Clone the repository**
   ```bash
   git clone https://github.com/FrereAlidor/Comparison_of_deep_learning_Tomato_Freshness_Stage_Recognition.git
   cd Comparison_of_deep_learning_Tomato_Freshness_Stage_Recognition
````

2. **Set up the environment**

   ```bash
   pip install -r requirements.txt
   ```

3. **Train a model**

   ```bash
   python train_yolov5m.py    # Or use train_xception.py / train_transformer.py
   ```

4. **Test / Evaluate**

   ```bash
   python evaluate_model.py
   ```

---

## 📌 Conclusion

This project demonstrates the efficiency of transformer-based models and YOLOv5m for classifying tomato freshness stages. While YOLOv5m is well-suited for real-time deployment, Transformer models offer the best accuracy.

---

## 📧 Contact

For any questions or collaboration inquiries, feel free to contact:

**Alidor MBAYANDJAMBE MASHEKE**
Email: [alidormbayandjambe@gmail.com](mailto:alidormbayandjambe@gmail.com)
GitHub: [FrereAlidor](https://github.com/FrereAlidor)

---

```

Let me know if you'd like a French version or to add badges, DOI for publication, or links to Colab notebooks or Hugging Face models.
```
