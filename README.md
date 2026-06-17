# Shelf Intelligence v2.0:  AI Powered Retail Shelf Analysis

**One reference image. One shelf photo. Instant analysis. Fully offline.**

<img width="1600" height="840" alt="VK_ShelfIntelligence_Medium_Cover(1)" src="https://github.com/user-attachments/assets/3b6532ba-a98b-4208-90b5-f9f2d133c2a0" />


[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/VK-Ant/Shelf-Intelligence-AI-Powered-Retail-Shelf-Analysis/blob/main/POC/ShelfIntelligence_v2.ipynb)

---

## What This Does

Upload a retail shelf photo and get structured analysis — products detected, brand share of shelf, stock levels, empty spots, and actionable recommendations. Upload a reference product image and the model finds that specific product on the shelf without any training data.

Built out of curiosity to solve a real-world retail problem using multimodal vision-language models.

---

## Features

| S.No. | Feature | Description |
|---|---------|-------------|
| 1 | Reference Image Matching | Upload one product photo, find it on any shelf |
| 2 | Text-Based Product Search | Type a product name, model locates it |
| 3 | Full Shelf Analysis | Products, brands, stock levels, shelf health score |
| 4 | Detection and Count | Precise per-shelf product count with facing numbers |
| 5 | Share of Shelf | Brand visibility percentage across entire shelf |
| 6 | Stock Level Estimation | High / Medium / Low per product |
| 7 | Empty Spot Detection | Identifies and locates shelf gaps |
| 8 | Planogram Compliance | Compare reference layout vs current shelf |
| 9 | Competition Analysis | Brand ranking with competitive insights |
| 10 | Restock Priority | Urgency ranking based on stock level and shelf share |

---

## Model Comparison

Tested on the same shelf images using free Colab T4 GPU (16GB VRAM).

| Model | Brand | Year | VRAM | JSON Quality | Speed | Best For |
|-------|-------|------|------|-------------|-------|----------|
| **Qwen2.5-VL-3B** | Alibaba | Jan 2025 | ~6GB | ★★★★☆ | ★★★☆☆ | Reliable structured output |
| **Qwen3-VL-2B** | Alibaba | Oct 2025 | ~4GB | ★★★★★ | ★★★★☆ | Best accuracy/size ratio |
| **Gemma 4 E4B** | Google | Apr 2026 | ~4GB | ★★★★☆ | ★★★★★ | Fastest inference |
| **Gemma 3n E4B** | Google | Jun 2025 | ~3GB | ★★★☆☆ | ★★★★★ | Smallest, mobile/edge ready |

Qwen excels at structured text extraction. Gemma excels at speed and brand recognition. Both run fully offline.

---

## Quick Start

1. Open the Colab notebook (click the badge above)
2. Select GPU runtime (Runtime → Change runtime type → T4 GPU)
3. Run all cells
4. Gradio UI launches with a public shareable link
5. Upload shelf image → click Analyze

No API keys. No setup. No cost.

---

## Why Most Shelf Intelligence Projects Fail

The $940M shelf intelligence market (Trax, ParallelDots, Infilect, Vispera, Neurolabs) has 53+ companies competing. Most projects still fail because of:

1. **Training data hunger** — traditional CV needs 500-1000 labeled images per SKU
2. **Field image quality** — blurry, angled, poorly lit photos break trained models
3. **Infrastructure cost** — cloud GPU at scale costs Rs 2-5 lakhs per month
4. **Data privacy** — shelf images contain competitive intelligence
5. **Long deployment cycles** — 3-6 months to implement

This approach uses multimodal VLMs that work with one reference image and zero training data. The customer already has a product photo.

---

## Key Insight

Clarity of frame matters more than the model. A clean, well-lit shelf photo gives 95%+ accuracy. A blurry phone photo at an angle gives 60%. The solution is not a better model — it is better capture guidance.

<img width="1757" height="752" alt="Screenshot 2026-06-17 085402" src="https://github.com/user-attachments/assets/cc6901fe-d481-4719-8737-e6d0a8979ef9" />

---

## Tech Stack

- **Models**: Qwen2.5-VL-3B / Qwen3-VL-2B / Gemma 4 E4B / Gemma 3n E4B
- **Runtime**: Google Colab (free T4 GPU)
- **UI**: Gradio with custom CSS
- **Dependencies**: transformers, torch, Pillow, gradio
- **Privacy**: 100% on-device processing, zero API calls

---

## Author

**Venkatkumar (VK)**
- GitHub: [@vk-ant](https://github.com/vk-ant)
- Medium: [@VK_Venkatkumar](https://medium.com/@VK_Venkatkumar)
- LinkedIn: [@VK_Venkatkumar](https://linkedin.com/in/VK-Venkatkumar)

---

## License

Apache2.0 — use it, modify it, build on it. Attribution appreciated.
