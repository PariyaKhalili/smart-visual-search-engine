🔍 Visual Search Engine using CLIP and ViT
This project implements a smart visual search engine using two powerful models:

CLIP (by OpenAI) for text-to-image search

ViT (Vision Transformer by torchvision) for image-to-image search

It uses CIFAR-10, a small image dataset, and FAISS for efficient similarity search. A modern Gradio web interface is included for interaction.

📸 Features
🔤 Text-based search using CLIP (e.g., "a red airplane")

🖼️ Image-based search using ViT (upload a query image)

🎨 Smooth Gradio UI with theme customizations

⚡ Fast similarity search using FAISS

📦 Compact dataset: CIFAR-10 (first 1000 images)

🧠 Models Used
Model	Usage	Source
CLIP (ViT-B/32)	Text-to-image embedding	OpenAI CLIP
ViT (vit_b_16)	Pure image embeddings	torchvision.models

🚀 Run Locally
1. Clone the repository
bash
Copy
Edit
git clone https://github.com/yourusername/visual-search-cifar10.git
cd visual-search-cifar10
2. Install dependencies
Make sure you have Python 3.8+ and then run:

bash
Copy
Edit
pip install -r requirements.txt
If requirements.txt is not available, install manually:

bash
Copy
Edit
pip install gradio torchvision faiss-cpu numpy tqdm pillow
pip install git+https://github.com/openai/CLIP.git
⚠️ For GPU support, install faiss-gpu and ensure PyTorch is installed with CUDA.

3. Run the app
bash
Copy
Edit
python app.py
The Gradio interface will launch in your browser at http://127.0.0.1:7860.

📁 Dataset Used
This project uses the CIFAR-10 dataset, loaded via torchvision.datasets. Only the first 1000 training images are used for faster indexing.

🖼️ Demo UI
The app lets you:

Choose CLIP or ViT

Enter a text prompt (CLIP)

Upload a query image (ViT)

View the top 6 similar images (with category labels)

📦 Project Structure
bash
Copy
Edit
├── app.py                 # Main script (or .ipynb if notebook)
├── README.md              # You are here!
├── requirements.txt       # Dependencies
├── assets/                # (optional) Screenshots or demos
📌 Screenshots (Optional)
You can include Gradio interface screenshots here if needed.

