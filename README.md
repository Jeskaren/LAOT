# LAOT: A Benchmark for Low-Light and Amodal Occlusion Tracking

[![License: CC BY-NC-SA 4.0](https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc-sa/4.0/)
[![Paper](https://img.shields.io/badge/Paper-arXiv-red)](https://arxiv.org/abs/xxxx.xxxxx)

**LAOT** (Low-light and Amodal Occlusion Tracking) is a challenging benchmark designed to evaluate object tracking algorithms under real-world visual degradation — specifically **low-light conditions** and **partial/full occlusion**. It is the first benchmark to combine both challenges in a standardized dataset and evaluation framework.

---

## 🚀 Highlights

- 🌙 **Low-Light Tracking**: Real-world sequences captured in dark environments with varying illumination.
- 🧱 **Amodal Occlusion Reasoning**: Frame-level occlusion annotations (including occlusion ratios).
- 🧪 **Fine-Grained Evaluation**: AP metrics under three occlusion levels: *No Occlusion*, *Partial Occlusion*, *Heavy Occlusion*.
- 🛠️ **Flexible Evaluation Code**: Python-based evaluation tools with IOU and occlusion analysis support.
- 📊 **21 Popular Trackers Evaluated**: Includes deep learning-based and traditional methods.

---

## 📁 Dataset Structure
LAOT/
├── seq/
│ ├── 0/
│ │ ├── images/
│ │ └── groundtruth.txt
│ ├── 1/
│ └── ...
├─────────────────


- `groundtruth.txt` format: `x, y, w, h, occlusion_level`  

---

## 📈 Evaluation
We provide a script to compute **Average Precision (AP)** under three occlusion categories:

| Occlusion Level   | Range       |
|-------------------|-------------|
| without Occlusion | 0.0 - 0.2   |
| Partial Occlusion | 0.2 - 0.8   |
| Heavy Occlusion   | 0.8 - 1.0   |


## 📊 Evaluation Results

The following table shows the AP accuracy of 21 tracking algorithms on the LAOT dataset under three occlusion levels:

| Algorithm     | Without Occlusion (8734) | Partial Occlusion (4486) | Heavy Occlusion (3190) |
|---------------|---------------------------|----------------------------|--------------------------|
| AQATrack      | 0.8342                    | 0.5999                     | 0.1489                   |
| ...           | ...                       | ...                        | ...                      |
| ZoomTrack     | 0.8264                    | 0.5854                     | 0.1680                   |

