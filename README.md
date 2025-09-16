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

📦 Dependencies

The following Python libraries are required:

torch
torchvision
pillow
numpy
tqdm
ipython
