# Synthetic Data Generation in the GenAI Era ✨

A small research project and presentation exploring how modern generative models create synthetic data and how this transforms traditional data mining workflows.

## Overview 📌

This repo bundles all artifacts from the project:

- 📝 A short paper based on the ACM tutorial by Li et al. (2025)
- 📊 Slide deck on synthetic data generation
- 🎥 Recorded presentation video
- 📰 Medium article aimed at a broader audience

The focus is on explaining **why synthetic data matters**, **how different generative models work**, and **what can go wrong** (model collapse) when synthetic data is misused.

## Contents 📂

- `paper/`  
  - `synthetic_data_gen_paper.pdf` – final written report
- `slides/`  
  - `Short_Story_presentation.pptx` – presentation slides
- `video/`  
  - `synthetic-data-presentation.mp4` – recorded talk (7–10 minutes)
- `scripts/`  
  - `presentation_script.md` – speaking notes used for the video
- `media/`  
  - Key diagrams and figures used in the slides
- `README.md`  
  - You are here


## Project Summary 🧠

- **Problem:**  
  Real-world data is scarce, expensive to label, and constrained by privacy and proprietary restrictions. This limits progress in data-hungry AI systems.

- **Core Generative Approaches:**  
  - **GANs:** Competitive generator–discriminator training; strong for images but prone to mode collapse.  
  - **Diffusion Models:** Noise-based forward and reverse process; more stable and diverse, now applied beyond images.  
  - **LLMs:** Autoregressive models that synthesize high-quality text and can be wrapped into data generation pipelines.

- **Notable Methods Covered:**  
  - **MagPie:** Template-driven LLM generation of alignment and instruction data.  
  - **DataGen:** Engineering-oriented pipeline with attribute control and RAG-based validation.  
  - **TabDDPM:** Diffusion for tabular data, balancing ML efficacy, privacy, and diversity.

- **Evaluation Dimensions:**  
  - **Fidelity** – How close synthetic data is to real data distributions.  
  - **Utility** – How well models trained on synthetic data perform on real test sets.  
  - **Privacy** – Protection against memorization of real records (e.g., DCR-style checks).  
  - **Diversity** – Coverage of rare cases and the full data manifold.

- **Model Collapse:**  
  Iteratively training models only on their own synthetic outputs leads to loss of rare patterns, amplified biases, and degraded performance. Mixing in fresh real data (“entropy injection”) is critical.

- **Applications:**  
  - 🏥 Healthcare – synthetic clinical records under HIPAA-style constraints.  
  - 💳 Finance – privacy-preserving fraud detection data.  
  - 🎓 Education – student performance modeling with limited real data.

## How to Use This Repo 🚀

- **Read the paper** if you want the structured, citation-heavy overview.  
- **View the slides** for a visual summary suitable for talks or teaching.  
- **Watch the video** for a compact, spoken explanation with diagrams.  
- **Check the Medium article** for a more narrative, accessible version of the same ideas.

You are welcome to reuse the slides or structure for your own study notes, course projects, or internal tech talks. Please cite the original ACM tutorial by Li et al. (2025) and the referenced papers if you build on this work.

## Medium Article 🔗

- Medium link: `https://medium.com/@jvithlani4/generative-models-for-synthetic-data-a-deep-dive-into-the-gen-ai-era-cbd5bcb77187?postPublishedType=initial`

The article is written for practitioners and students who are comfortable with machine learning basics and want intuition for when and how to use synthetic data safely.

## Acknowledgements 🙏

- Based on: **Li et al., “Generative Models for Synthetic Data: Transforming Data Mining in the GenAI Era” (ACM tutorial, 2025)**  
- Plus key works on GANs, diffusion models, MagPie, DataGen, TabDDPM, model collapse, and related methods.

😊
