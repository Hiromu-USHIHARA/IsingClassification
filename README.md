# 🧠 Ising Phase Classifier: CNN-based 2D Ising Model Phase Detection

This project demonstrates a simple convolutional neural network (CNN) to classify spin configurations of the 2D Ising model into **ordered (low-temperature)** and **disordered (high-temperature)** phases based only on visual spin patterns.

<p align="center">
  <img src="assets/spin_example.png" alt="Spin configuration example" width="250"/>
  <img src="assets/transition_plot.png" alt="Phase transition prediction" width="400"/>
</p>

---

## 🔬 Motivation

Phase transitions are fundamental in physics. This demo shows that a CNN can detect the phase transition of the 2D Ising model **without explicit knowledge of physical quantities** such as energy or magnetization — it learns directly from spin images.

---

## 🚀 Try it in Google Colab

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](
https://colab.research.google.com/github/your-username/ising-phase-classifier/blob/main/demo.ipynb)

> You can generate spin configurations at various temperatures and let the model predict the phase!

---

## 📁 Repository Contents

| File | Description |
|------|-------------|
| `ising_model.py` | Contains Ising model simulation (Metropolis method) and model definition |
| `model.h5` | Pretrained model (optional: can be trained in Colab too) |
| `demo.ipynb` | Google Colab-compatible notebook for demonstration |
| `assets/` | Sample spin images and output graphs |
| `requirements.txt` | Library dependencies (not needed in Colab) |

---

## 🧪 Example Output

### Spin Configurations

At low and high temperatures:

<p align="center">
  <img src="assets/spin_lowT.png" alt="Low T" width="200"/>
  <img src="assets/spin_highT.png" alt="High T" width="200"/>
</p>

### Model Prediction across Temperatures

<p align="center">
  <img src="assets/transition_plot.png" alt="Transition Plot" width="400"/>
</p>

---

## 🧰 Technologies Used

- Python (NumPy, Matplotlib)
- TensorFlow / Keras
- Google Colab

---

## 📌 Notes

- The model is trained in a **supervised** fashion using temperature-based labels.
- Future work may include **unsupervised detection of the phase transition** using clustering or dimensionality reduction.

---

## 📜 License

MIT License.
