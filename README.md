# RAISA Dataset Release

This page provides a **partial public release** of the dataset used in RAISA performance evaluation.

---

## 1. What is Released

### 1) Obstacle images (public)
- **40 real obstacle images** captured by the author
- **320 augmented variants**
- **Total: 360 images**

📁 Path: <a href="https://drive.google.com/file/d/10KpeBKiI0glV_Brfv_v1Z97SzXIVcUuN/view?usp=drive_link" target="_blank" rel="noopener">Download link</a>


### 2) Scenario-level Ground Truth (GT) sentences (public)
We release **GT sentences** for:
- **Train Driver (Operator) instruction**
- **Traffic controller (Dispatcher) instruction**

📁 Paths:
- `gt/gt_train_driver.md`
- `gt/gt_traffic_controller.md`

> Note:
> We do **not** redistribute image frames extracted from online videos due to copyright restrictions.
> Instead, we only provide the source video URLs and the number of extracted frames.
> We only release **textual GT** prepared by the author.


### 3) Online video sources (links-only) and manual scenario labeling

Due to copyright restrictions, we do **not** redistribute image frames extracted from online videos.
Instead, we provide **only the source video URLs and the number of extracted frames**.

**Data collection procedure.** Frames were **not collected per scenario** at the time of extraction.
We first extracted frames from each source video following a uniform sampling policy; therefore, the **number of extracted frames varies by video length**.
We then **manually assigned scenario labels** by inspecting each extracted frame.

**Sampling policy.** For each source video, we sampled frames at **1-minute intervals**.
Within each 1-minute window, we randomly selected one timestamp and extracted the corresponding frame.
As a result, extracted timestamps are not aligned to exact minute marks (e.g., 00:15, 01:02, 02:38, ...).

> “# Extracted frames” denotes the number of image frames extracted **from the corresponding source video** and used in our internal evaluation.

| Source ID | URL | # Extracted frames |
|---|---|---:|
| 001 | https://www.youtube.com/watch?v=_L2H5-jE6ts | 483 |
| 002 | https://www.youtube.com/watch?v=tqjx4Hu8KpY | 1533 |
| 003 | https://www.youtube.com/watch?v=3m0wMrvvbs0&list=PLS58inbn9oJXjEnsaZvJZVfrjbwE0VQ2B | 452 |
| 004 | https://www.youtube.com/watch?v=i0E41L7pxzY | 634 |
| 005 | https://www.youtube.com/watch?v=aBXW4uEurns | 587 |
| 006 | https://www.youtube.com/watch?v=zCoCOHOYd28 | 736 |
| 007 | https://www.youtube.com/watch?v=Mw9qiV7XlFs | 354 |
| 008 | https://www.youtube.com/watch?v=L-O0k1oF9_Y | 727 |
| 009 | https://www.youtube.com/watch?v=5E2ycdUi2m8&list=PLWoUS6jbUY-ovODHQBDkvR4w-W9ARQmRT | 1626 |
| 010 | https://www.youtube.com/watch?v=wVCaef0oZmQ | 285 |
| 011 | https://www.youtube.com/watch?v=x8ez4XNT080 | 651 |
| 012 | https://www.youtube.com/watch?v=w-4BP8MRuis | 645 |
| 013 | https://www.youtube.com/watch?v=-ZWiyFtyBrs&list=PLqVXtaI0Orw6z3e7q2fe16IE1KsPbbilZ&index=5 | 717 |
| 014 | https://www.youtube.com/watch?v=UPKpH0YvGeI&list=PLqVXtaI0Orw6z3e7q2fe16IE1KsPbbilZ&index=6 | 649 |
| 015 | https://www.youtube.com/watch?v=jGpt3Nvnqis&list=PLqVXtaI0Orw6z3e7q2fe16IE1KsPbbilZ&index=7 | 695 |
| 016 | https://www.youtube.com/watch?v=xvhvhtxzbrQ&list=PLqVXtaI0Orw6z3e7q2fe16IE1KsPbbilZ&index=10 | 589 |
| 017 | https://www.youtube.com/watch?v=9j7aGqhHffo&list=PLqVXtaI0Orw6z3e7q2fe16IE1KsPbbilZ&index=18 | 600 |
| 018 | https://www.youtube.com/watch?v=aweycDW7eLE&list=PLqVXtaI0Orw7aXSlJQWfXCT46MDgvgqmp&index=4 | 543 |
| 019 | https://www.youtube.com/watch?v=G2nTCr5spQY&list=PLWoUS6jbUY-pwPC1C397w8BoG-0bMqr_o&index=5 | 321 |
| 020 | https://www.youtube.com/watch?v=WmeZnG-nDhk&list=PLq9tAKxg4w28e9Dw5f8qcCclGjoXbFT9y&index=43 | 51 |
| 021 | https://www.youtube.com/watch?v=XdU3W2IOdBw  | 14 |
| 022 | https://www.youtube.com/watch?v=ukOHqdPbYYg | 117 |
| 023 | https://www.youtube.com/watch?v=pphgq49lslI | 324 |


---


## 2. Dataset Format

### 2.1 Obstacle image naming
- Real: `track_obstacle_##.jpg`
- Augmented: `track_obstacle_##_<augtype>.jpg`

### 2.2 GT sentence structure
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

## 3. Intended Use / Not Intended Use

### Intended use
- RAISA evaluation and reproducible benchmarking on railway safety instruction generation
- Research on vision-language reasoning and scenario-conditioned instruction generation

### Not intended use
- Surveillance, biometric identification, or privacy-invasive applications

---

## 4. Citation

Please cite our paper if you use this dataset:

**RAISA Paper (under review; working title)**  
- Title (working): *RAISA: A Vision-based Intelligent Safety Guidance Agent for Safer Railway Operations via Modular Prompt-Orchestrated Reasoning*  
- Authors: Kyung Ho Kang, Kyoung Ok Yang, and Jun Won Choi  
- Venue/Year: Under review, 2026  
- DOI/URL: To appear

---

## 5. License

- Obstacle images + GT sentences: CC BY 4.0
- See `LICENSE`.

---

## 6. Contact
- Maintainer: KYUNGHO KANG
- Email: khkang@spa.hanyang.ac.kr

---

“No privacy-invasive use (e.g., identification of individuals) is permitted.”
