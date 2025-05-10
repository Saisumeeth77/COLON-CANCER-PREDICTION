<h1 align="center">Colon Cancer Prediction</h1>

<div align= "center">
  <h4>Colon Cancer Prediction using ResNet-50.</h4><br>
 </div>
 
# Overview
This colon cancer prediction project involves building an image-based classification model using histopathological images of colon tissue. The aim is to develop a robust and accurate deep learning model that assists in early cancer detection and diagnosis. By leveraging convolutional neural networks (CNNs), the project helps pathologists identify malignant tissues more efficiently, improving clinical workflows and patient outcomes—especially critical in the post-COVID-19 healthcare environment, where diagnostic automation can reduce workload and enhance precision.

# Dataset Description
The study utilizes the LC25000 dataset, which contains histopathological images of lung and colon tissues. For this project, only the Colon Adenocarcinoma (cancerous) and Normal Colon (non-cancerous) classes are used. The dataset is divided into training, validation, and test sets to ensure proper generalization and unbiased evaluation.

To maintain classification accuracy and fairness, the dataset is balanced between the two classes. Preprocessing steps include resizing images (e.g., 224×224), normalization, data augmentation, and the removal of redundant or corrupted images. The LC25000 dataset is widely recognized for its applicability in deep learning-based medical image classification tasks.

• Sample of different tissue types in dataset

![image](Outputs/image_sets.jpg)

# Some Screenshots

• Heatmap overlays highlighting Frequency of tumor types.<br>

![image](Outputs/tumor-typre.jpg)

# Methodology
1. Data Preprocessing: Image resizing, normalization, and augmentation.
2. Model Development: Building and training different CNN models including basic CNN and pre-trained architectures.
3. Evaluation Metrics: Accuracy, Precision, Recall, and F1-score, Grad-Cam, ROC-AUC.
4. Visualization: Confusion matrix and training/validation accuracy plots.

# Model Used
• ResNet-50

# Model Evaluation

| Class | Precision | Recall | F1 Score | Support |
| ----------- | ----------- | ----------- | ----------- | ----------- |
| 0 | 0.94 | 0.84 | 0.89 | 500 |
| 1 | 0.86 | 0.95 | 0.90 | 500 |
| Accuracy | 0.92(1000 samples) |
| Macro Avg | 0.90 | 0.90 | 0.90 | 1000 |
| Weighted Avg | 0.90 | 0.90 | 0.90 | 1000 |

![image](Outputs/report.jpg)

<h1 align="center">Confusion Matrix</h1>

![image](Outputs/confusion-matrix.jpg)

<h1 align="center">Model Accuracy</h1>

![image](Outputs/model-acc.jpg)

# Conclusion
This study proposes a deep learning approach for detecting colon cancer using histopathological images from the LC25000 dataset. The CNN-based model accurately distinguishes between adenocarcinoma and normal tissue, aided by preprocessing and hyperparameter tuning. Results highlight strong performance and support the use of explainable AI in medical diagnostics, though challenges like false positives remain.
