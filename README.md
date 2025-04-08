# ML4DQMEvaluationTask

Vision Transformer
This project uses a Vision Transformer (ViT) to classify calorimeter images (64x72) from two datasets into two groups.

#### Architecture
Model: Vision Transformer (ViT)
Splits images into 8x8 patches (72 patches total).
6 layers, 8 attention heads, 128 embedding size.
No pre-training, built from scratch.
#### Dataset
Custom data from Run357479_Dataset_iodic.npy (label 0) and Run355456_Dataset_jqkne.npy (label 1), normalized to 0-1.
#### Training
Loss: Binary Cross-Entropy with Logits.
Optimizer: AdamW (learning rate: 0.0001).
Batch size: 32, 25 epochs, random horizontal/vertical flips.


#### Results
Model	Accuracy	AUC-ROC Score
ViT	1.000	1.000

#### Visuals
![image](https://github.com/user-attachments/assets/6eb7d6fe-e177-4027-8c77-499049f2867f)
