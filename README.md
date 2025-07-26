# Comparison of Deep Learning Models for Tomato Freshness Stage Recognition

This project presents a comparative study of three deep learning models — **YOLOv5m**, **Xception**, and a **Vision Transformer** — for classifying tomato freshness stages: **Fresh**, **At-risk**, and **Rotten**. A mobile application is also included for real-time deployment.

## Mobile App Demo

Watch our mobile application in action as it detects and classifies tomato freshness stages in real-time:

[![Demo Video](./thumbnail.jpg)](https://github.com/FrereAlidor/Comparison_of_deep_learning_Tomato_Freshness_Stage_Recognition/releases/download/v1.0/Video_demo_application.mp4)

[Click here to watch or download the demo video](https://github.com/FrereAlidor/Comparison_of_deep_learning_Tomato_Freshness_Stage_Recognition/releases/download/v1.0/Video_demo_application.mp4)

## Dataset

The dataset used in this project contains images grouped into three categories:

- **Fresh**: Healthy tomatoes ready for consumption
- **At-risk**: Tomatoes showing early signs of deterioration
- **Rotten**: Tomatoes that are no longer suitable for consumption

Images were preprocessed and augmented to improve model robustness under varying lighting and environmental conditions.

## Trained Models

We trained and compared the following deep learning models:

- **YOLOv5m**: Real-time object detection model
- **Xception**: CNN architecture optimized for image classification
- **Vision Transformer (ViT)**: Transformer-based model for image understanding

## Performance Comparison

| Model | Metric | At-risk (%) | Fresh (%) | Rotten (%) | Overall Accuracy (%) | Training Time | Prediction Time/Image |
|-------|--------|-------------|-----------|------------|---------------------|---------------|----------------------|
| **YOLOv5m** | Accuracy | 98.33 | 100.00 | 100.00 | **99.44** | 2h 33m | 156.1 ms |
| | Precision | 98.33 | 100.00 | 100.00 | | | |
| | Recall | 98.33 | 100.00 | 100.00 | | | |
| | F1-score | 99.15 | 100.00 | 99.17 | | | |
| **Xception** | Accuracy | 99.00 | 98.25 | 98.72 | 98.67 | 1h 46m | 762.0 ms |
| | Precision | 97.70 | 98.60 | 99.68 | | | |
| | Recall | 99.00 | 98.25 | 98.72 | | | |
| | F1-score | 98.35 | 98.42 | 99.20 | | | |
| **Transformer** | Accuracy | 100.00 | 99.00 | 99.00 | **99.56** | 4h 40m | 33.9 ms |
| | Precision | 99.12 | 99.72 | 99.67 | | | |
| | Recall | 98.83 | 99.48 | 99.39 | | | |
| | F1-score | 98.97 | 99.60 | 99.53 | | | |

## Mobile Application

The Android mobile app was developed using the **YOLOv5m** model to provide real-time predictions. Users can capture or upload images of tomatoes and receive instant freshness classification results.

## Repository Structure

```
.
├── Application_detector/           # Contains APK and source code for mobile app
├── All_file_model/                 # Notebooks and scripts for all models
│   ├── final_project_200_tomato_Xception_Final.ipynb
│   ├── final_tomato_class_2.ipynb
│   ├── tomato_swin200s_old.ipynb
│   ├── train.py / val.py / detect.py / tutorial.ipynb
├── Data/                           # Training and validation datasets
├── Video_demo_application.mp4      # Demo video (linked above)
├── README.md                       # This file
└── ...
```

## Installation & Usage

### 1. Clone the repository
```bash
git clone https://github.com/FrereAlidor/Comparison_of_deep_learning_Tomato_Freshness_Stage_Recognition.git
cd Comparison_of_deep_learning_Tomato_Freshness_Stage_Recognition
```

### 2. Install dependencies
```bash
pip install -r requirements.txt
```

### 3. Train a model
```bash
python train.py   # Adjust for YOLOv5, Xception, or Transformer
```

### 4. Evaluate the model
```bash
python val.py
```

## Key Findings

- **Vision Transformer** achieved the highest overall accuracy at 99.56%
- **YOLOv5m** offers the best balance between accuracy (99.44%) and inference speed (156.1 ms)
- **Xception** provides solid performance with moderate training time but slower inference
- All models demonstrate excellent performance for practical deployment

## Conclusion

This project demonstrates the effectiveness of **Transformer-based models** and **YOLOv5m** in detecting tomato freshness. While Transformers offer the highest accuracy, YOLOv5m provides the best performance for real-time deployment scenarios.

## Contact

For questions, feedback, or collaboration inquiries:

**Alidor MBAYANDJAMBE MASHEKE**  
Email: [alidormbayandjambe@gmail.com](mailto:alidormbayandjambe@gmail.com)  
GitHub: [FrereAlidor](https://github.com/FrereAlidor)

## License

This project is available under the MIT License. See the LICENSE file for more details.



