# CPD-MMRS
Official PyTorch implementation of "Contrastive Parameter Disentanglement for Multi-modal Remote Sensing Image Generation"
<div align="center">

<h1> Contrastive Parameter Disentanglement for Multi-modal Remote Sensing Image Generation </h1>

<br>

<!-- 彩色标签 (Badges) -->
<a href="https://pytorch.org/"><img src="https://img.shields.io/badge/PyTorch-v1.8+-red.svg?logo=PyTorch" alt="PyTorch"></a>
<a href="https://www.python.org/"><img src="https://img.shields.io/badge/Python-3.8+-blue.svg?logo=python" alt="Python"></a>
<a href="#"><img src="https://img.shields.io/badge/Paper-Under_Review-green.svg?logo=arxiv" alt="Paper"></a>

</div>

<br>

## 📣 News
- **[Latest]** The official PyTorch source code and pre-trained models will be released immediately upon acceptance. Please stay tuned!

---

## 📖 Abstract
Remote sensing image generation is a pivotal technique for mitigating image scarcity in earth observation. However, existing generation methods are confined to single-modality synthesis, thereby failing to harness the complementary information inherent in multimodal images. In this paper, we propose a text-to-multimodal remote sensing image generation task, which aims to generate semantically and structurally consistent multimodal remote sensing images (e.g., optical, infrared, and synthetic aperture radar) from a single textual prompt. The core challenge of this task lies in mapping invariant semantics from a single text prompt while adapting to different modality attributes. We observe that LoRA adapters exhibit an inherent functional dichotomy, enabling disentanglement of semantic invariance and modality attributes at the parameter level. Thus, we propose a contrastive parameter disentanglement module that establishes the parameter-level disentanglement of shared semantics and distinct attributes within the orthogonal core subspace. Based on this, we next build a disentangled optimization strategy that first constrains the matrix A of the LoRA adapter to extract invariant semantics by multi-modal contrastive objective and then guides the multiple matrices B to adapt different modality attributes under text prompts, thereby enabling the simultaneous generation of semantically consistent multimodal images. Furthermore, to guarantee structure consistency in generated multi-modal images, we then devise a query-key structure transfer mechanism that injects structural correlation priors from the anchor modality into other modalities during the inference process. Extensive experiments demonstrate that our proposed method outperforms state-of-the-art remote sensing image generation methods in terms of generation quality and semantic consistency, and also yields superior performance in the downstream remote sensing object classification task.

---

## 🖼️ Visual Results (WHU-OPT-SAR) Dataset

<!-- 下面这行的 src 里面换成你在GitHub上传的那张大图的真实链接 -->
<p align="center">
  <img src="https://github.com/DUT-ZYu/CPD-MMRS/blob/main/1_06.jpg" alt="CPD-MMRS Results" width="100%">
</p>
<p align="center">
  <em>Qualitative comparison of the generated effects of our CPD-MMRS model</em>
</p>

## 🖼️ Visual Results (OSI) Dataset 

<!-- 下面这行的 src 里面换成你在GitHub上传的那张大图的真实链接 -->
<p align="center">
  <img src="https://github.com/DUT-ZYu/CPD-MMRS/blob/main/1_07.jpg" alt="CPD-MMRS Results" width="100%">
</p>
<p align="center">
  <em>Qualitative comparison of the generated effects of our CPD-MMRS model</em>
</p>

<p align="center">
  <img src="https://github.com/DUT-ZYu/CPD-MMRS/blob/main/1_08.jpg" alt="CPD-MMRS Results" width="100%">
</p>
<p align="center">
  <em>Qualitative comparison of the generated effects of our CPD-MMRS model</em>
</p>

<p align="center">
  <img src="https://github.com/DUT-ZYu/CPD-MMRS/blob/main/1_09.jpg" alt="CPD-MMRS Results" width="100%">
</p>
<p align="center">
  <em>Qualitative comparison of the generated effects of our CPD-MMRS model</em>
</p>
...

## 🚀 Getting Started (Code Coming Soon)

### Prerequisites
- Linux or windows
- Python 3.11+
- PyTorch 2.1+
- CUDA 12.0+
