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

## 📁 Dataset Download

📥  [Download LAOT Dataset on Google Drive](https://drive.google.com/file/d/1EVXtmeZcQzit3vFS_aY6z_nHdfoqTuD1/view?usp=drive_link)

📥  [Download LAOT Dataset on Quark Drive](https://pan.quark.cn/s/685605e1289c)


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
| ARTrack       | 0.8055                    | 0.6179                     | 0.2505                   |
| AVTrack       | 0.7375                    | 0.4394                     | 0.1276                   |
| DCPT          | 0.7787                    | 0.5288                     | 0.1455                   |
| DropTrack     | 0.8382                    | 0.6355                     | 0.1730                   |
| HiFT          | 0.6616                    | 0.3567                     | 0.0928                   |
| HIPTrack      | 0.8540                    | 0.6355                     | 0.2176                   |
| ODTrack       | 0.8056                    | 0.6638                     | 0.2567                   |
| OStrack       | 0.7899                    | 0.5671                     | 0.1708                   |
| Procontext    | 0.8414                    | 0.6268                     | 0.1903                   |
| ROMTrack      | 0.7825                    | 0.5497                     | 0.1295                   |
| SeqTrack      | 0.8243                    | 0.5791                     | 0.1602                   |
| SGLATrack     | 0.7226                    | 0.4545                     | 0.1107                   |
| SiamAPN++     | 0.7124                    | 0.4019                     | 0.1386                   |
| SiamCAR       | 0.7228                    | 0.4050                     | 0.1116                   |
| SiamGAT       | 0.6883                    | 0.4454                     | 0.1414                   |
| SimTrack      | 0.8286                    | 0.5798                     | 0.1530                   |
| SLGTrack      | 0.7226                    | 0.4545                     | 0.1107                   |
| Stark         | 0.7035                    | 0.3796                     | 0.0784                   |
| UncTrack      | 0.8247                    | 0.6547                     | 0.2417                   |
| ZoomTrack     | 0.8264                    | 0.5854                     | 0.1680                   |


