# 🖼️ Text-to-Image Generation with GLIDE + CLIP

This repository contains an implementation of **GLIDE** (Guided Language to Image Diffusion for Generation and Editing) with **CLIP-based guidance** for text-to-image generation.  
It takes a **text prompt** and produces **high-resolution (256×256) images** by first generating a low-resolution sample and then upscaling it with an upsampler model.

---

## 🚀 Features
- Generate images from any text description.
- Uses **CLIP guidance** to align images with the text prompt.
- Supports **GPU acceleration (CUDA)** for faster sampling.
- Produces **64×64 → 256×256 upsampled images**.
- Easy to modify for different prompts, batch sizes, and sampling steps.

---

## 📂 Repository Structure
📦 glide-text2im-project/
├── 📄 clip_guided_notebook.ipynb # Main Colab notebook implementation
├── 📄 README.md # Project documentation
└── 📁 samples/ # Generated images 

---

### 🛠️ Technologies Used
- **Programming Language:** Python 3  
- **Libraries & Frameworks:**
  - **PyTorch** → Deep learning framework for model loading & inference  
  - **GLIDE (OpenAI Glide-Text2IM)** → Text-to-Image generation model  
  - **HuggingFace Transformers / Diffusers** → For handling pretrained models and pipelines  
  - **PIL (Python Imaging Library)** → Image processing and display  
  - **IPython.display** → Displaying images in Jupyter/Colab  
- **Tools:**
  - Google Colab / Jupyter Notebook for execution  
  - GitHub for version control and project hosting  
  - CUDA (if GPU available) for faster model inference  
---
