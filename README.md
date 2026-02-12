# Scalable and Lightweight ViT-Tiny forMixed-Defect Classification in Semiconductor Wafer Maps
Semiconductor wafer defect classification is critical for ensuring high precision and yield in manufacturing. Traditional CNN-based models often struggle with class imbalances and recognition of the multiple overlapping defect types in wafer maps. To address these challenges, we propose ViT-Tiny, a lightweight Vision Transformer (ViT) framework optimized for wafer defect classification. Trained on the WM-38k dataset. ViT-Tiny outperforms its ViT-Base counterpart and state-of-the-art (SOTA) models, such as MSF-Trans and CNN-based architectures. Through extensive ablation studies, we determine that a patch size of 16 provides optimal performance. ViT-Tiny achieves an F1-score of 98.4%, surpassing MSF-Trans by 2.94% in four-defect classification, improving recall by 2.86% in two-defect classification, and increasing precision by 3.13% in three-defect classification. Additionally, it demonstrates enhanced robustness under limited labeled data conditions, making it a computationally efficient and reliable solution for real-world semiconductor defect detection. Manuscript https://arxiv.org/abs/2504.02494


![image](https://github.com/user-attachments/assets/4a101e7b-5235-4ccf-b05c-16a5c167c123)

## ViT Model Variants 
| Model     | Layers | Hidden Size | Attention Heads | MLP Size | Params|  
| :---      | :---:  | :---:       | :---:           |  :---:   |  ---: |
| ViT-Tiny  | 12     | 192         | 3               | 768      | ~5.7M |
| ViT-Small | 12     | 384         | 6               | 1536     | ~22M  |
| ViT-Base  | 12     | 768         | 12              | 3072     | ~86 M |


