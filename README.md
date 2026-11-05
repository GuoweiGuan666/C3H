# C3H: Compression-to-Consensus Criteria Hijacking in Multimodal LLM Recommender Systems

**NeurIPS 2026 · Main Track (Poster)**

**Guowei Guan · Yurong Hao · Jiaming Zhang · Fuyao Zhang · Wei Yang Bryan Lim**  
College of Computing and Data Science, Nanyang Technological University, Singapore

[**Paper (OpenReview PDF)**](https://openreview.net/pdf?id=QEtoKLRzjN)

---

## Overview

Multimodal large language model (MLLM) recommenders use an item's text and images to decide what to recommend. **C3H** studies a targeted, inference-time item-promotion attack in which a seller edits the content of a **single item**, without access to the victim's parameters, gradients, training data, or query feedback.

C3H exploits a *compression-to-consensus (C2C)* ranking preference: cues that remain salient after input compression and are supported across text and images may have greater influence on candidate ranking. The attack uses public pretrained encoders to select promising cues, then performs constrained text and image edits designed to preserve semantic and visual plausibility.

## Key Features

- **Strict zero-query setting:** no victim-model queries during attack construction.
- **Single-item scope:** only the target item's text and image are edited.
- **Cross-modal cue selection:** public encoders guide the choice of textual and visual cues.
- **Constrained content editing:** a stealthiness gate checks fidelity and image–text coherence, with a clean-content fallback.
- **Evaluation across architectures:** experiments use VIP5 and Qwen2-VL-2B-Instruct on MicroLens-100K, Amazon Beauty, and Amazon Sports.

## Code Release

> **Status: In preparation — source code is not yet publicly available.**

This repository is currently the public project page for the paper. We plan to add the implementation, configuration files, and reproduction instructions here. Until those files are uploaded, this repository is **not** a complete reproduction package.

## Citation

If you find the work useful, please cite:

```bibtex
@inproceedings{guan2026c3h,
  title     = {C3H: Compression-to-Consensus Criteria Hijacking in Multimodal LLM Recommender Systems},
  author    = {Guan, Guowei and Hao, Yurong and Zhang, Jiaming and Zhang, Fuyao and Lim, Wei Yang Bryan},
  booktitle = {Advances in Neural Information Processing Systems},
  year      = {2026}
}
```

## Responsible Use

This project is intended to support research on the security and robustness of AI recommender systems.
