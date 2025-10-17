# Crop Disease Classification: Traditional ML vs Deep Learning

## Links
Youtube: 
Report Document: https://docs.google.com/document/d/16r5Dfw4OJ2K4spKBho5rQgXGiZ-4ybKwrNCECf0dHl4/edit?usp=sharing 

## 🌱 Project Overview

This project addresses the critical issue of **hunger caused by insufficient crop consumption due to crop diseases** that reduce harvest yields. We develop machine learning models to classify healthy and diseased leaves, demonstrating the application of both traditional machine learning and deep learning approaches in the agricultural sector.

## 🎯 Problem Statement

Crop diseases are a major threat to global food security, causing significant yield losses that contribute to hunger and food insecurity. Early detection and classification of plant diseases can help farmers take preventive measures, reduce crop losses, and improve food production.

## 🔬 Technical Approaches

### 1. Traditional Machine Learning
- **Feature Engineering**: Color histograms, texture features, statistical measures
- **Models Implemented**:
  - Logistic Regression
  - Random Forest Classifier
  - Support Vector Machine (SVM)
- **Feature Scaling**: StandardScaler for normalization

### 2. Deep Learning
- **Architecture**: Convolutional Neural Network (CNN)
- **Layers**: 3 Conv2D + MaxPooling layers, Dense layers with Dropout
- **Input**: Raw images (128x128x3)
- **Optimization**: Adam optimizer with binary cross-entropy loss

## 📈 Experiment Results

| Model | Type | Accuracy | Parameters | Dataset |
|-------|------|----------|------------|---------|
| Logistic Regression | Traditional ML | ~0.85 | Default sklearn | Engineered Features |
| Random Forest | Traditional ML | ~0.88 | n_estimators=100 | Engineered Features |
| SVM | Traditional ML | ~0.87 | Default sklearn | Engineered Features |
| CNN | Deep Learning | ~0.92 | 3 Conv layers, Dropout 0.5 | Raw Images |


### Quick Start
1. Update dataset path in Cell 2 of the notebook
2. Run all cells sequentially
3. View results in the experiment table and visualizations

## 🔍 Key Findings

### Performance Insights
- **CNN outperformed traditional ML** by ~4-7% accuracy
- **Random Forest showed best traditional ML performance** due to handling feature interactions
- **Color and texture features** were most discriminative for traditional ML

### Agricultural Impact
- **Early detection**: Models can identify diseases before visible symptoms spread
- **Cost reduction**: Automated monitoring reduces manual inspection costs
- **Yield preservation**: Timely intervention can save 20-40% of crop yields

## 🛠️ Model Evaluation

### Metrics Used
- Accuracy
- Confusion Matrix
- Validation/Test split performance

### Error Analysis
- Common misclassifications between early-stage diseases and healthy leaves
- Lighting conditions and image quality affected traditional ML more than CNN
- CNN showed better generalization to varied leaf orientations

## 🌟 Future Enhancements

1. **Multi-class Classification**: Extend to specific disease types (blight, rust, mildew)
2. **Real-time Deployment**: Mobile app for field use
3. **Transfer Learning**: Leverage pre-trained models (ResNet, EfficientNet)
4. **Data Augmentation**: Expand dataset with synthetic samples
5. **Explainable AI**: Visualize which leaf regions indicate disease

## 🤝 Contributing

We welcome contributions from the community! Areas for contribution:
- Additional model architectures
- Dataset expansion
- Performance optimization
