# RAISA Dataset Release (Obstacle 360 + Scenario GT)

This page provides a **partial public release** of the dataset used in RAISA performance evaluation.

---

## 1. What is Released

### 1) Obstacle images (public)
- **40 real obstacle images** captured by the author
- **320 augmented variants**
- **Total: 360 images**

📁 Path: `data/obstacle_public/`


### 2) Scenario-level Ground Truth (GT) sentences (public)
We release **GT sentences** for:
- **Driver (train operator) instruction**
- **Dispatcher (traffic controller) instruction**

📁 Paths:
- `gt/driver_gt.md`
- `gt/dispatcher_gt.md`

> Note:
> We do **not** redistribute image frames extracted from online videos due to copyright restrictions.
> Instead, we only provide the source video URLs and the number of extracted frames.
> We only release **textual GT** prepared by the author.

---

## 2. Download / Access

### Direct folder browsing on GitHub
- Obstacle images: `data/obstacle/`
- GT sentences:
  - Driver GT: `gt/driver_gt.md`
  - Dispatcher GT: `gt/dispatcher_gt.md`

> If the repository becomes large, consider enabling Git LFS for images.

---

## 3. Dataset Format

### 3.1 Obstacle image naming (recommended)
We recommend the following naming rule (you may adjust):
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

## 4. GT Sentences (Embedded View)

Below are **embedded views** of the GT sentence files.

### 4.1 Train Driver GT
- File: [`gt/driver_gt.md`](../gt/driver_gt.md)

<details>
<summary>Click to expand (Driver GT)</summary>

> ⚠️ For single-page maintenance, you can paste the full driver GT content here.  
> Otherwise, keep it in `gt/driver_gt.md` and leave this block as a link-only section.

</details>

### 4.2 Traffic Controller GT
- File: [`gt/dispatcher_gt.md`](../gt/dispatcher_gt.md)

<details>
<summary>Click to expand (Dispatcher GT)</summary>

> ⚠️ For single-page maintenance, you can paste the full dispatcher GT content here.  
> Otherwise, keep it in `gt/dispatcher_gt.md` and leave this block as a link-only section.

</details>

---

## 5. Intended Use / Not Intended Use

### Intended use
- RAISA evaluation and reproducible benchmarking on railway safety instruction generation
- Research on vision-language reasoning and scenario-conditioned instruction generation

### Not intended use
- Surveillance, biometric identification, or privacy-invasive applications

---

## 6. Citation

Please cite our paper if you use this dataset:

**RAISA Paper**  
- Title: RAISA: A Vision-based Intelligent Safety Guidance Agent for Safer Railway Operations via Modular Prompt-Orchestrated Reasoning
- Authors: Kyung Ho Kang, Kyoung Ok Yang, AND Jun Won Choi
- Venue/Year: (TODO)
- DOI/URL: (TODO)

---

## 7. License

- Obstacle images + GT sentences: CC BY 4.0
- See `LICENSE`.

---

## 8. Contact
- Maintainer: KYUNGHO KANG
- Email: khkang@spa.hanyang.ac.kr

---

“This repository does not redistribute frames extracted from online videos; only obstacle images and author-written GT sentences are provided.”

“No privacy-invasive use (e.g., identification of individuals) is permitted.”
