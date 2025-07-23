This Python script (task2.py) uses Stable Diffusion via Hugging Face’s diffusers library to generate realistic AI images from text prompts. It is designed to run in Google Colab or any Python environment with CUDA-enabled GPU support.
Features
Uses Stable Diffusion v1.4 and v1.5 models.

Generates high-quality images from custom text prompts.

Saves and displays the generated image using PIL.

GPU acceleration via CUDA for faster performance.

Supports multiple prompts in a single run. 
 Installation
Before running the script, make sure the following libraries are installed:
pip install diffusers
pip install transformers
pip install torch
pip install accelerate
pip install safetensors
How It Works
Load a pre-trained model
The script supports both CompVis/stable-diffusion-v1-4 and runwayml/stable-diffusion-v1-5 models from Hugging Face.

Device Handling
Automatically uses GPU (cuda) if available; otherwise, falls back to CPU.

Text Prompt
You can customize the prompt to generate different scenes. Example:
prompt = "A quiet path in a moss-covered forest after rain, wet leaves, puddles reflecting trees, natural soft light, DSLR quality"
Image Generation & Saving
The image is generated from the prompt and saved locally:
image.save("generated_image.png")
Display
In Colab or Jupyter environments, the image is displayed inline:
display(image)
