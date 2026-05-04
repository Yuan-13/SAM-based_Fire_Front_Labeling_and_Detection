# Boundary-Oriented Fire Front Localization (SFL & SFD)

This repository accompanies our paper:

**"Revisiting Fire Front Localization: A Boundary-Oriented Framework for Labeling and Detection in Aerial Imagery"**  
(under review at ISPRS Journal of Photogrammetry and Remote Sensing)

---

## 🔍 Overview

Accurate fire front localization in aerial wildfire imagery is challenging due to irregular, open, and partially observable fire structures. Instead of modeling fire regions, we reformulate the task as a **boundary-oriented problem**, explicitly targeting thin and open fire front boundaries.

This repository presents two complementary components:

- **SFL (SAM-based Fire Front Labeling)**  
  A semi-automatic annotation framework for generating high-quality fire front boundaries from aerial imagery. It leverages Meta's **Segment Anything Model (SAM)** with minimal user interaction to produce accurate, consistent, and reproducible one-pixel-wide masks.

- **SFD (SAM-based Fire Front Detection)**  
  A boundary-oriented detection framework for localizing fire front boundaries from aerial imagery. It leverages **Segment Anything Model (SAM)** to identify boundary subsets anchored on adjacent unburned regions, producing accurate, stable, and one-pixel-wide predictions with strong data efficiency.

---

## 🧰 SFL: Annotation Tool

We provide an interactive online annotation tool:

👉 https://huggingface.co/spaces/YF13/SFL

### Usage

- Upload image(s)
- Select prompt points and fire front ranges
- Generate **one-pixel-wide fire front mask**
- Visualize overlay and refine if needed
- Export mask and overlay

### Example

![SFL Demo](assets/sfl_demo.png)

### Alternative workflow
Manual selection can be performed using tools such as LabelMe, followed by processing with our SFL pipeline (to be released).

---

## 🔥 SFD: Fire Front Detection

### Example

![SFD Demo](assets/sfd_demo.png)

---

### ⭐ Key Characteristics

- Boundary-oriented formulation
- Data-efficient
- Robust across modalities and datasets
- Consistent performance under boundary-oriented evaluation metrics

---

## 🖼️ Examples

We provide qualitative examples including:

- Input aerial wildfire imagery
- SFL-generated boundary labels
- SFD predictions
- Overlay visualizations

See: `examples/`

---

## ⚙️ Environment

- Python 3.10+
- PyTorch
- Segment Anything Model (SAM)

Detailed setup and dependencies will be provided upon release.

---

## 📦 Availability

- **Code**: Full implementation (training and evaluation) will be released upon acceptance of the paper.  
- **Annotation Tool (SFL)**: Publicly available at the link above.

---

## 📘 Citation

If you find this work useful, please cite:

```bibtex
@article{***2026,
title={Revisiting Fire Front Localization: A Boundary-Oriented Framework for Labeling and Detection in Aerial Imagery},
author={Anonymous},
journal={Under Review},
year={2026}
}

---

## 📄 License

To be specified upon release.

