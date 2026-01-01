# RAISA Dataset Release (Obstacle 360 + Scenario GT)

This page provides a **partial public release** of the dataset used in RAISA performance evaluation.

---

## 1. What is Released

### 1) Obstacle images (public)
- **40 real obstacle images** captured by the author
- **320 augmented variants**
- **Total: 360 images**

📁 Path: `data/obstacle/`


### 2) Scenario-level Ground Truth (GT) sentences (public)
We release **GT sentences** for:
- **Train Driver (Operator) instruction**
- **Traffic controller (Dispatcher) instruction**

📁 Paths:
- `gt/driver_gt.md`
- `gt/dispatcher_gt.md`

> Note:
> We do **not** redistribute image frames extracted from online videos due to copyright restrictions.
> Instead, we only provide the source video URLs and the number of extracted frames.
> We only release **textual GT** prepared by the author.


### 3) Online video sources (links-only)
We provide **only the source video URLs and the number of extracted frames** (no frame redistribution).

| Source ID | URL | Scenario label(s) | # Extracted frames | Notes |
|---|---|---|---:|---|
| YT-001 | (paste URL) | Daytime (clear) | TODO | (optional) sampling rule / segment |
| YT-002 | (paste URL) | Nighttime (clear) | TODO |  |
| YT-003 | (paste URL) | Tunnel driving | TODO |  |
| YT-004 | (paste URL) | Railway signal ahead | TODO |  |
| YT-005 | (paste URL) | Approaching platform | TODO |  |
| YT-006 | (paste URL) | Foggy weather | TODO |  |
| YT-007 | (paste URL) | Rainy weather | TODO |  |
| YT-008 | (paste URL) | Snowy weather | TODO |  |
| YT-009 | (paste URL) | Mixed / Multiple | TODO | (optional) dominant label policy |

---

## 2. Download / Access

### Direct folder browsing on GitHub
- Obstacle images: `data/obstacle/`
- GT sentences:
  - Driver GT: `gt/driver_gt.md`
  - Dispatcher GT: `gt/dispatcher_gt.md`

---

## 3. Dataset Format

### 3.1 Obstacle image naming
- Real: `OBS_###_REAL.jpg`
- Augmented: `OBS_###_AUG_<augtype>.jpg`

### 3.2 GT sentence structure
GT is organized by scenario labels:
- Daytime (clear weather)
- Nighttime (clear weather)
- Tunnel driving
- Railway signal ahead
- Approaching platform
- Foggy weather
- Rainy weather
- Snowy weather
- Obstacle

---

## 4. Intended Use / Not Intended Use

### Intended use
- RAISA evaluation and reproducible benchmarking on railway safety instruction generation
- Research on vision-language reasoning and scenario-conditioned instruction generation

### Not intended use
- Surveillance, biometric identification, or privacy-invasive applications

---

## 5. Citation

Please cite our paper if you use this dataset:

**RAISA Paper**  
- Title: RAISA: A Vision-based Intelligent Safety Guidance Agent for Safer Railway Operations via Modular Prompt-Orchestrated Reasoning
- Authors: Kyung Ho Kang, Kyoung Ok Yang, AND Jun Won Choi
- Venue/Year: (TODO)
- DOI/URL: (TODO)

---

## 6. License

- Obstacle images + GT sentences: CC BY 4.0
- See `LICENSE`.

---

## 8. Contact
- Maintainer: KYUNGHO KANG
- Email: khkang@spa.hanyang.ac.kr

---

“No privacy-invasive use (e.g., identification of individuals) is permitted.”
