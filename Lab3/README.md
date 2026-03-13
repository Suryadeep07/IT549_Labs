Lab 3 Assignment
Image-Based AQI Classification using CNN and Pretrained Models

Name: Suryadeepsinh Gohil
ID: 202301463

Lab Details:
In this lab we use deep learning to guess the Air Quality Index (AQI) class just by looking at pictures of different places. The code covers data setup, model building, training, and testing.

Model Details:
We built and tested two models using only the image data and the target labels.
1. Basic CNN: A simple, custom model built from scratch with 3 convolutional blocks.
2. ResNet18 (Transfer Learning): A strong, pre-trained model. We froze the early layers to save time and trained the deeper layers to learn the specific AQI images.

Here is how the two models performed on the test data:

| Model | Accuracy | Precision | Recall | F1-Score |
| :--- | :---: | :---: | :---: | :---: |
| Basic CNN (Scratch) | 0.6533 | 0.6574 | 0.6533 | 0.6419 |
| ResNet18 (Transfer) | 0.9644 | 0.9648 | 0.9644 | 0.9645 |

Conclusion: The ResNet18 model did a much better job than the Basic CNN. Since ResNet18 was already trained on millions of images, it already knew how to see shapes, edges, and colors. This transfer learning helped it score 96.44% accuracy, while the scratch model only scored 65.33%.
