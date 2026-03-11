<h1 align="center">
  <br>
  <img width="300" src="./core/http/static/logo.png"> <br>
  <strong>tecmarco10 / Core-Inference-Engine</strong>
<br>
</h1>

<p align="center">
  <img src="https://img.shields.io/badge/Status-Active_Development-green?style=for-the-badge" alt="Status"/>
  <img src="https://img.shields.io/badge/License-MIT-yellow.svg?style=for-the-badge" alt="License"/>
  <img src="https://img.shields.io/badge/Focus-Local_AI_Inference-blue?style=for-the-badge" alt="Focus"/>
</p>

> [!IMPORTANT]
> **Core-Inference-Engine** is a private-to-public migration project focusing on providing a free, Open Source OpenAI alternative for local environments. This repository consolidates months of local research into a unified, drop-in replacement REST API.

---

## 💻 Project Overview

This engine acts as a drop-in replacement REST API compatible with OpenAI specifications for local AI inferencing. It allows you to run Large Language Models (LLMs), generate images, and process audio locally on consumer-grade hardware.

### 🚀 Key Features
- **Zero-GPU Requirement:** Optimized for CPU-only environments but supports full GPU acceleration.
- **Model Agnostic:** Compatible with GGUF, GGML, and Transformers formats.
- **Multi-Modal Support:** Handles Text-to-Speech (TTS), Speech-to-Text (STT), and Image Generation.
- **API Compatible:** Seamlessly works with existing tools that expect OpenAI endpoints.

## 🛠️ Supported Backends

| Category | Backend Engine |
|----------|----------------|
| **Text** | llama.cpp, vLLM, transformers, MLX |
| **Audio** | whisper.cpp, faster-whisper, moonshine |
| **Image** | stablediffusion.cpp, diffusers |

## ⚙️ Quickstart (Docker)

To initiate the core engine on your local infrastructure:

```bash
# CPU optimized build
docker run -ti --name ai-core -p 8080:8080 tecmarco10/core-engine:latest
