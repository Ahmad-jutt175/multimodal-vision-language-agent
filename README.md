# 🤖 Multi-Modal Vision-Language AI Agent

**MNC-Grade Advanced AI Project | Resume Portfolio**

---

## 📌 Project Overview

A hybrid AI framework that combines **Computer Vision (CV)** and **Natural Language Processing (NLP)** for autonomous scene understanding — inspired by systems used in Tesla FSD, Microsoft Azure AI Vision, and xAI Grok.

The agent can:
- 👁️ **See** an image and describe what it contains (Image Captioning)
- 🧠 **Answer questions** about a visual scene (Visual Question Answering)
- 🔗 **Fuse** vision + language context to make decisions (Multi-Modal Reasoning)
- 📊 **Log** all predictions with timestamps (Production-style Inference Logging)

---

## 🏗️ Architecture

```
Input Image ──► Vision Encoder (ViT) ──┐
                                        ├──► Fusion Layer ──► Text Output
User Query  ──► Text Tokenizer (BERT) ──┘    (BLIP Model)
```

---

## 📂 Folder Structure

```
multimodal-vision-language-agent/
│
├── config/
│   └── model_config.json          # Model hyperparameters & dataset references
│
├── data/
│   └── sample_scene.jpg           # Auto-downloaded during notebook run
│
├── notebooks/
│   ├── 01_environment_setup.ipynb # Library installation & verification
│   └── 02_multimodal_inference_pipeline.ipynb  # Main pipeline
│
├── outputs/
│   └── predictions_log.txt        # Auto-generated inference logs
│
├── README.md
└── requirements.txt
```

---

## 🔗 Datasets Used

| Dataset | Source | Purpose |
|---------|--------|---------|
| **Flickr8k** | [Kaggle](https://www.kaggle.com/datasets/adityajn105/flickr8k) | Image captioning benchmark |
| **COCO 2017** | [Kaggle](https://www.kaggle.com/datasets/awsaf49/coco-2017-dataset) | Object detection & scene understanding |

---

## 🛠️ Models Used

- **BLIP** (Bootstrapping Language-Image Pre-training) by Salesforce Research
- **Vision Transformer (ViT)** backbone for image encoding
- **BERT-style** text encoder for language understanding

---

## 🚀 How to Run

```bash
# 1. Install dependencies
pip install -r requirements.txt

# 2. Run notebooks in order:
# notebooks/01_environment_setup.ipynb  →  Verify installation
# notebooks/02_multimodal_inference_pipeline.ipynb  →  Run AI agent
```

---

## Bullet Points

- Developed a **hybrid Multi-Modal AI framework** combining Computer Vision and NLP for autonomous scene understanding
- Integrated pre-trained **Vision-Language Transformers (BLIP architecture)** via Hugging Face and PyTorch for image captioning and Visual Question Answering (VQA)
- Engineered an **inference pipeline** converting spatial feature maps into structured textual descriptions with production-style logging
- Benchmarked against **Flickr8k and COCO 2017** datasets (industry-standard benchmarks used by Microsoft and Meta)
- Optimized **multi-modal data fusion** through conditional context injection and beam search decoding

---

*Built with ❤️ using Hugging Face Transformers, PyTorch, and OpenCV*
