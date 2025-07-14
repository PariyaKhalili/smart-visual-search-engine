# 🔍 Visual Search Engine using CLIP and ViT
This project implements a smart visual search engine for both prompt and image input using two powerful models:

* CLIP (by OpenAI) for text-to-image search

* ViT (Vision Transformer by torchvision) for image-to-image search

It uses CIFAR-10, a small image dataset, and FAISS library for efficient similarity search. A modern Gradio web interface is included for interaction:
![Example](https://github.com/PariyaKhalili/smart-visual-search-enginr/blob/main/assets/app_ui.jpg)

✨ Features
1. Text-based search using CLIP (e.g., "a red airplane")

2. Image-based search using ViT (upload a query image)

3. Smooth Gradio UI with costomized theme

4. Fast similarity search using FAISS

5. Compact dataset of CIFAR-10 (first 2000 images)

6. Error handeling with an empty prompt

7. The app UI changes by choosing either CLIP or ViT 

🧠 Models Used
Model	Usage	Source
CLIP (ViT-B/32)	Text-to-image embedding	OpenAI CLIP
ViT (vit_b_16)	Pure image embeddings	torchvision.models

## 🎥 Demo
Click the link below to watch the demo:
[Demo](assets/demo.mp4)
