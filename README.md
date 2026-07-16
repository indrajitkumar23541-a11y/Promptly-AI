# Promptly-AI: Next-Gen AI Image Generation Studio 🎨

![Build Status](https://img.shields.io/badge/Build-Passing-brightgreen)
![Python](https://img.shields.io/badge/Python-3.10%2B-blue)
![License](https://img.shields.io/badge/License-MIT-green)
![Framework](https://img.shields.io/badge/Framework-Gradio-orange)

> **Promptly AI** is a powerful, highly customizable, and user-friendly web interface for generating stunning AI images. Powered by Stable Diffusion and Gradio, it offers an intuitive dashboard for both beginners and advanced AI artists to create, edit, and upscale synthetic media locally.

---

## 📸 Interface Preview

![Promptly AI Interface](screenshot.png)
*(A sleek Gradio-based interface for effortless image generation)*

---

## 🌟 Feature Overview

### 🖌️ Core Generation Modes
- **Text-to-Image (txt2img):** Generate high-fidelity images from text prompts with precise seed control.
- **Image-to-Image (img2img):** Transform existing images using AI-guided styling and masking.
- **Inpainting & Outpainting:** Seamlessly edit specific parts of an image or expand its borders beyond the original frame.

### 🧠 Advanced AI Tools
- **Textual Inversion:** Train and use custom embeddings to teach the AI new concepts or art styles with minimal VRAM.
- **Attention Control:** Emphasize or de-emphasize specific words in your prompt using syntax like `(keyword:1.2)`.
- **Prompt Matrix & X/Y/Z Plots:** Generate multi-dimensional comparison grids to test different prompts, samplers, and seeds simultaneously.

### 🔍 Upscaling & Face Restoration
- **Neural Upscalers:** Integrated support for RealESRGAN, ESRGAN, SwinIR, and LDSR for crystal-clear resolution scaling.
- **Face Fixers:** Built-in GFPGAN and CodeFormer models to automatically repair and restore faces in AI-generated portraits.

---

## 🏗️ Architecture & Tech Stack

**Promptly AI** is built on a robust Python backend with a reactive frontend:

| Component | Technology | Role |
|-----------|------------|------|
| **Core Engine** | PyTorch / Stable Diffusion | Deep learning image synthesis |
| **Frontend** | Gradio | Web-based interactive user interface |
| **Backend** | Python 3.10+ | API routing, model loading, and hardware acceleration |

### Request Flow
```text
┌─────────────────┐       ┌─────────────────┐       ┌─────────────────┐
│                 │       │                 │       │                 │
│  User Interface │ ────▶ │  Python Backend │ ────▶ │ PyTorch / CUDA  │
│  (Gradio Web)   │       │  (launch.py)    │       │ (Stable Diff.)  │
│                 │ ◀──── │                 │ ◀──── │                 │
└─────────────────┘       └─────────────────┘       └─────────────────┘
```

---

## 🚀 Getting Started

### Prerequisites
- **Python 3.10.6+** (Add to PATH during installation)
- **Git**
- An NVIDIA GPU with CUDA support (Recommended for fast generation, though CPU fallback exists).

### Installation

1. **Clone the Repository**
   ```bash
   git clone https://github.com/indrajitkumar23541-a11y/Promptly-AI.git
   cd Promptly-AI
   ```

2. **Run the Application**
   - **Windows:** Double-click `webui-user.bat`
   - **Linux/Mac:** Run `./webui.sh` in the terminal

   *Note: On the first run, the script will automatically create a virtual environment (`venv`) and download all necessary dependencies and base models.*

3. **Access the Studio**
   Once the terminal displays `Running on local URL:  http://127.0.0.1:7860`, open that link in your web browser!

---

## 👨‍💻 Author

**Created and Developed by Indrajit Kumar**

- **GitHub:** [indrajitkumar23541-a11y](https://github.com/indrajitkumar23541-a11y)
- **Email:** indrajitkumar23541@gmail.com

---

## 📄 License

This project is licensed under the MIT License — see the [LICENSE.txt](LICENSE.txt) file for details.

*Promptly AI — Turning imagination into pixels.*
