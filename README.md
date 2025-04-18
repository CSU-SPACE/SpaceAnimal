# 🧪 SpaceAnimal Evaluation Tools

Evaluation tools for pose estimation and tracking of model organisms such as **C. elegans**, **zebrafish**, and **Drosophila** in spaceflight experiments.

---

## 📌 Pose Estimation Evaluation

### 🔧 Installation

1. Install `xtcocotools`:
   ```bash
   pip install xtcocotools
   ```

2. Install additional dependencies and the package:
   ```bash
   pip install -r requirements.txt
   python setup.py install
   ```

### ⚙️ Sigma Settings

Set the `sigma` values according to the target species:

- **C. elegans (worm)**:
  ```python
  [0.25, 0.75, 0.75, 0.75, 0.25]
  ```

- **Zebrafish**:
  ```python
  [1.25, 1.25, 1.25, 1.55, 1.55, 1.35, 1.35, 1.35, 1.35, 1.25]
  ```

- **Drosophila (fruit fly)**:
  ```python
  [0.35, 0.55, 0.55, 0.75, 0.75, 0.55, 0.62, 0.62, 0.55, 0.62, 0.62, 0.55,
   0.62, 0.62, 0.55, 0.62, 0.62, 0.55, 0.62, 0.62, 0.55, 0.62, 0.62, 0.55,
   0.87, 0.87]
  ```

---

## 🚶 Pose Tracking Evaluation

### 🔧 Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/CSU-SPACE/SpaceAnimal.git
   ```

2. Install the evaluation tool dependencies:
   ```bash
   cd SpaceAnimal/eval_tools
   pip install -r requirements.txt
   ```

### ▶️ Evaluation Example

Run the evaluation with example data:
```bash
python eval_tools/evalpose/evaluate.py \
  -g eval_tools/examples/posetrack_gts/ \
  -p eval_tools/examples/posetrack_preds/ \
  -c worm \
  -o eval_tools/out
```

> Replace `worm` with `zebrafish` or `fly` to evaluate other species.

---

## 🙏 Acknowledgement

This evaluation framework is built upon the [poseval](https://github.com/leonid-pishchulin/poseval) repository by **Leonid Pishchulin**.

---

## 📫 Contact

For issues or questions, please open an issue or contact the authors through the [GitHub repository](https://github.com/CSU-SPACE/SpaceAnimal).
