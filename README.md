# Text-to-Image Generation with GLIDE and CLIP Guidance

This repository explores text-conditioned image generation using **GLIDE** with **CLIP-based guidance**. The notebook demonstrates a prompt-to-image workflow and an upsampling stage.

The implementation is available in `clip_guided.ipynb`.

## Overview

Text-to-image generation maps a natural-language description to a generated image. This project combines:

- **GLIDE** — a text-conditioned diffusion model for image generation.
- **CLIP guidance** — a vision-language similarity signal used to encourage alignment between generated imagery and a text prompt.
- **Upsampling** — a higher-resolution stage in the generation workflow.

The notebook is the source of truth for the exact model checkpoints, sampling configuration, dependencies, and output dimensions.

## Generation workflow

```text
Text prompt
    |
    v
GLIDE text-conditioned generation
    |
    v
CLIP-guided sampling
    |
    v
Upsampling stage
    |
    v
Generated image
```

## Technologies

- Python
- PyTorch
- GLIDE
- CLIP
- PIL / image utilities
- Jupyter Notebook or Google Colab
- CUDA-compatible GPU (where available)

## Run the notebook

1. Clone this repository.
2. Open `clip_guided.ipynb` in Jupyter or Google Colab.
3. Review the notebook for the required model checkpoints and dependency versions.
4. Install the dependencies specified by the notebook.
5. Follow the notebook cells to load the models, provide a prompt, and run generation.

A CUDA-enabled runtime is recommended for practical inference speed. Memory requirements depend on the selected checkpoints, sampling settings, and image resolution.

## Notes and limitations

- Generated images may contain visual artifacts or fail to represent all details in a prompt.
- CLIP similarity guidance is not a guarantee of semantic correctness or factual accuracy.
- Model checkpoints and dependencies may require separate downloads and may be subject to their own licenses and usage terms.
- Generation quality and runtime depend on the model configuration and compute environment.

## Repository contents

- `clip_guided.ipynb` — notebook containing the generation workflow.

---

Built by [Nuaima Saeed](https://github.com/Nuaima).
