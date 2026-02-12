# Scalable and Lightweight ViT-Tiny forMixed-Defect Classification in Semiconductor Wafer Maps
Semiconductor wafer defect classification is critical for ensuring high precision and yield in manufacturing. Traditional CNN-based models often struggle with class imbalances and recognition of the multiple overlapping defect types in wafer maps. To address these challenges, we propose ViT-Tiny, a lightweight Vision Transformer (ViT) framework optimized for wafer defect classification. Trained on the WM-38k dataset. ViT-Tiny outperforms its ViT-Base counterpart and state-of-the-art (SOTA) models, such as MSF-Trans and CNN-based architectures. Through extensive ablation studies, we determine that a patch size of 16 provides optimal performance. ViT-Tiny achieves an F1-score of 98.4%, surpassing MSF-Trans by 2.94% in four-defect classification, improving recall by 2.86% in two-defect classification, and increasing precision by 3.13% in three-defect classification. Additionally, it demonstrates enhanced robustness under limited labeled data conditions, making it a computationally efficient and reliable solution for real-world semiconductor defect detection. Manuscript https://arxiv.org/abs/2504.02494


![image](https://github.com/user-attachments/assets/4a101e7b-5235-4ccf-b05c-16a5c167c123)

## ViT Model Variants 
| Model     | Layers | Hidden Size | Attention Heads | MLP Size | Params|  
| :---      | :---:  | :---:       | :---:           |  :---:   |  ---: |
| ViT-Tiny  | 12     | 192         | 3               | 768      | ~5.7M |
| ViT-Small | 12     | 384         | 6               | 1536     | ~22M  |
| ViT-Base  | 12     | 768         | 12              | 3072     | ~86 M |


# ViT-Tiny for Semiconductor Wafer Defect Classification

![Accuracy](https://img.shields.io/badge/Accuracy-98.41%25-brightgreen)
![Parameters](https://img.shields.io/badge/Parameters-5.7M-blue)
![Inference](https://img.shields.io/badge/Inference-8.3ms-orange)
![License](https://img.shields.io/badge/License-MIT-yellow)

> 🏆 **State-of-the-art** wafer defect classification with **15× fewer parameters** than ViT-Base

## 📈 Performance Highlights

| Metric | ViT-Tiny (Ours) | Best Baseline | Improvement |
|--------|-----------------|---------------|-------------|
| Validation Accuracy | **98.41%** | 97.48% (Swin) | **+0.93pp** |
| Parameters | **5.7M** | 86M (ViT-Base) | **15× smaller** |
| Inference Speed | **8.3ms** | 14.7ms (Swin) | **1.77× faster** |
| GPU Memory | **412MB** | 1,843MB (Swin) | **4.47× less** |
| Training Time | **2.5 hrs** | 8.3 hrs (ViT-Base) | **3.3× faster** |
