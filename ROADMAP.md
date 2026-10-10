# AI/ML Project Roadmap

*22 projects · 8 categories · followed in a spiral order · beginner → advanced*
*Building toward embedded systems + AI/computer vision engineering roles*

**Progress:** 5 / 22 complete · Round 1: 2 of 6 done · **Next up:** 4.1 Build mini-GPT

**Legend:** ✅ Done &nbsp;·&nbsp; 🔄 In progress &nbsp;·&nbsp; ⬜ Not started &nbsp;·&nbsp; R1/R2/R3 = spiral round

### How this is organized
- **Categories** (below) group projects by topic. **The spiral order** (at the bottom) is the order they're built in.
- Round 1 builds a base in every category. Later rounds go deeper only where it pays off, so rounds get smaller.
- Every project after round 1 reuses something concrete from an earlier one — code, a model, or an evaluation habit.
- Foundations and Classical ML are exercise-style projects, grouped into one repo per category ([ML-Foundation](https://github.com/Altster/ML-Foundation), [Classical-ML](https://github.com/Altster/Classical-ML)). Everything else is a substantial build with its own repo.
- Every repo has a README covering the problem, the key decision, results, and how to run it.

---

<details open>
<summary><strong>1 — Foundations</strong> &nbsp;(3/3 done) &nbsp;→&nbsp; <a href="https://github.com/Altster/ML-Foundation">ML-Foundation</a></summary>
<br>

| # | Project | Status | Round | Focus | Stack | Repo |
|---|---------|:------:|:-----:|-------|-------|------|
| 1.1 | No-magic neural net (cat classifier) | ✅ | — | Backprop by hand in pure NumPy | NumPy, matplotlib | [ML-Foundation/1](https://github.com/Altster/ML-Foundation/tree/main/1.%20Cat%20Classifier%20Using%20a%20Shallow%20Neural%20Network) |
| 1.2 | Titanic oracle | ✅ | — | Feature engineering, sklearn pipelines, CV, Optuna, SHAP | pandas, scikit-learn, XGBoost | [ML-Foundation/2](https://github.com/Altster/ML-Foundation/tree/main/2.%20Titanic%20Oracle%20-%20Comparing%207%20ML%20models%20in%20predicting%20survival) |
| 1.3 | Cats vs dogs CNN + Mission control | ✅ | — | CNN from scratch, W&B tracking, Bayesian sweeps, transfer learning | PyTorch, W&B | [ML-Foundation/3](https://github.com/Altster/ML-Foundation/tree/main/3.%20Cat%20vs%20Dog%20Classifier%20CNN%2C%20Weights%20%26%20Biases%2C%20ResNet-18) |

</details>

<details open>
<summary><strong>2 — Classical ML</strong> &nbsp;(1/3 done) &nbsp;→&nbsp; <a href="https://github.com/Altster/Classical-ML">Classical-ML</a></summary>
<br>

| # | Project | Status | Round | Focus | Stack | Repo |
|---|---------|:------:|:-----:|-------|-------|------|
| 2.1 | Algorithm wars | ✅ | R1 | 8 algorithm families × 3 datasets, reusable comparison harness | scikit-learn, XGBoost | [Classical-ML/1](https://github.com/Altster/Classical-ML/tree/main/1.%20Algorithm%20War%20%28Comparative%20Analysis%20of%20Classical%20ML%20Algorithms%29) |
| 2.2 | Card fraud detective | ⬜ | R2 | Extreme imbalance, PR-AUC, cost-based thresholds, calibration | LightGBM, CatBoost, SHAP | *Classical-ML/2* |
| 2.3 | Signal forecaster | ⬜ | R3 | Time series: walk-forward validation, classical vs boosting vs foundation forecasters | statsforecast, LightGBM | *Classical-ML/3* |

</details>

<details open>
<summary><strong>3 — Computer Vision</strong> &nbsp;(1/4 done)</summary>
<br>

| # | Project | Status | Round | Focus | Stack | Repo |
|---|---------|:------:|:-----:|-------|-------|------|
| 3.1 | AI eye doctor | ✅ | R1 | Retinopathy grading, two-stage transfer learning, QWK, Grad-CAM | PyTorch, Albumentations, W&B | [AI-Eye-Doctor](https://github.com/Altster/AI-Eye-Doctor) |
| 3.2 | Arm's-eye view | ⬜ | R2 | Real-time detection + gesture control driving a robotic arm | YOLO26, MediaPipe, OpenCV, ONNX | *Arms-Eye-View* |
| 3.3 | Green screen killer v2 | ⬜ | R3 | U-Net from scratch vs a zero-shot foundation segmenter | PyTorch, segmentation-models-pytorch, Gradio | *Green-Screen-Killer* |
| 3.4 | ViT, short | ⬜ | R3 | Vision Transformer built from my own GPT blocks | PyTorch, timm | *ViT-From-Scratch* |

</details>

<details open>
<summary><strong>4 — Language & Transformers</strong> &nbsp;(0/4 done)</summary>
<br>

| # | Project | Status | Round | Focus | Stack | Repo |
|---|---------|:------:|:-----:|-------|-------|------|
| 4.1 | Build mini-GPT | ⬜ | R1 | GPT from scratch: tokenizer, attention, sampling, KV-cache | PyTorch, tiktoken, W&B | *Mini-GPT* |
| 4.2 | Three-way text classifier | ⬜ | R2 | TF-IDF vs fine-tuned encoder vs zero-shot LLM | HF transformers, Claude API | *Three-Way-Classifier* |
| 4.3 | AI study buddy | ⬜ | R2 | RAG over my notes, built around a hand-made eval set | sentence-transformers, ChromaDB, Gradio | *RAG-Study-Buddy* |
| 4.4 | AI intern | ⬜ | R3 | Research agent as a plain Python loop, with an MCP tool | Claude API, MCP, FastAPI | *AI-Research-Agent* |

</details>

<details open>
<summary><strong>5 — Unsupervised & Representation Learning</strong> &nbsp;(0/1 done)</summary>
<br>

| # | Project | Status | Round | Focus | Stack | Repo |
|---|---------|:------:|:-----:|-------|-------|------|
| 5.1 | Map of meaning + factory inspector | ⬜ | R1 | Embeddings, PCA/t-SNE/UMAP, clustering; autoencoder vs foundation-feature anomaly detection | scikit-learn, UMAP, PyTorch, timm | *Map-Of-Meaning* |

</details>

<details open>
<summary><strong>6 — Generative AI</strong> &nbsp;(0/2 done)</summary>
<br>

| # | Project | Status | Round | Focus | Stack | Repo |
|---|---------|:------:|:-----:|-------|-------|------|
| 6.1 | Noise to numbers | ⬜ | R1 | VAE → DDPM diffusion on the same small U-Net | PyTorch, W&B | *Noise-To-Numbers* |
| 6.2 | Straight lines | ⬜ | R2 | Flow matching vs DDPM, then a miniature latent generator | PyTorch, cleanfid | *Flow-Matching* |

</details>

<details open>
<summary><strong>7 — Reinforcement Learning</strong> &nbsp;(0/3 done)</summary>
<br>

| # | Project | Status | Round | Focus | Stack | Repo |
|---|---------|:------:|:-----:|-------|-------|------|
| 7.1 | Maze master → stick figure walks | ⬜ | R1 | Q-learning and REINFORCE from scratch, then PPO on continuous control | NumPy, Gymnasium, stable-baselines3 | *RL-Foundations* |
| 7.2 | **Track hunter** 🏁 | ⬜ | R2 | Deep RL racing agent in Trackmania, trained to beat human times (major project) | PyTorch, SAC, Openplanet, custom Gymnasium env | *Track-Hunter* |
| 7.3 | Reasoning trainer | ⬜ | R3 | LoRA + GRPO with verifiable rewards on a small LLM | HF TRL, PEFT | *Reasoning-Trainer* |

</details>

<details open>
<summary><strong>8 — Capstone</strong> &nbsp;(0/2 done)</summary>
<br>

| # | Project | Status | Round | Focus | Stack | Repo |
|---|---------|:------:|:-----:|-------|-------|------|
| 8.1 | Stand on giants | ⬜ | Cap | Reproduce a 2025–26 arXiv paper on limited compute | PyTorch, W&B | *Paper-Reproduction* |
| 8.2 | The arm that learns | ⬜ | Cap | Imitation learning on my own robotic arm from recorded demos | PyTorch, LeRobot, OpenCV | *Arm-That-Learns* |

</details>

---

## Build order

| Step | Project | Round | Status |
|:---:|---------|:-----:|:------:|
| — | 1.1–1.3 Foundations | — | ✅ |
| — | 2.1 Algorithm wars | R1 | ✅ |
| — | 3.1 AI eye doctor | R1 | ✅ |
| 1 | 4.1 Build mini-GPT | R1 | ⬜ ← next |
| 2 | 5.1 Map of meaning + factory inspector | R1 | ⬜ |
| 3 | 6.1 Noise to numbers | R1 | ⬜ |
| 4 | 7.1 Maze master → stick figure walks | R1 | ⬜ |
| | *Checkpoint 1 — base in every category* | | |
| 5 | **7.2 Track hunter** 🏁 | R2 | ⬜ |
| 6 | 2.2 Card fraud detective | R2 | ⬜ |
| 7 | 3.2 Arm's-eye view | R2 | ⬜ |
| 8 | 4.2 Three-way text classifier | R2 | ⬜ |
| 9 | 6.2 Straight lines | R2 | ⬜ |
| 10 | 4.3 AI study buddy | R2 | ⬜ |
| | *Checkpoint 2* | | |
| 11 | 2.3 Signal forecaster | R3 | ⬜ |
| 12 | 3.3 Green screen killer v2 | R3 | ⬜ |
| 13 | 3.4 ViT, short | R3 | ⬜ |
| 14 | 7.3 Reasoning trainer | R3 | ⬜ |
| 15 | 4.4 AI intern | R3 | ⬜ |
| | *Checkpoint 3* | | |
| 16 | 8.1 Stand on giants | Cap | ⬜ |
| 17 | 8.2 The arm that learns | Cap | ⬜ |

*Repo names in italics are planned and don't exist yet. Zillow killer and Traffic spy from the old plan were dropped in v5: Zillow overlapped with earlier projects, and Traffic spy's object detection now lives inside 3.2 Arm's-eye view.*
