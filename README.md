# **Medina Landmark Classification: ViT Fine-Tuning & LoRA**
This project focuses on building an advanced image classification model to recognize historical landmarks in Medina. By leveraging the Vision Transformer (ViT) architecture, the project demonstrates two powerful strategies to adapt a pre-trained model to a custom dataset.

# **Project Overview**
The core of this project is the Vision Transformer (ViT) model, originally pre-trained on the massive ImageNet-21k dataset. We explore two different approaches to fine-tune it for our specific task:

# 1. Full Fine-Tuning (Small & Large Datasets)
In this approach, we retrain all layers of the model. We experiment with different data scales—both Small and Large datasets—to observe how the amount of data impacts the model's ability to learn specific architectural features of Medina's landmarks.

# 2. Parameter-Efficient Fine-Tuning (PEFT) via LoRA
To make training faster and more resource-efficient, we implement LoRA (Low-Rank Adaptation). Instead of updating the entire model, we:
Freeze the original pre-trained weights.
Add small, trainable Adapters (rank decomposition matrices).
Significantly reduce memory usage and training time while maintaining high accuracy.


