# 🗣️ Automatic Speech Recognition for Badaga using HuBERT and Wav2Vec2.0

This project presents the first end-to-end Automatic Speech Recognition (ASR) system for **Badaga**, a low-resource Dravidian language spoken in the Nilgiris region of Tamil Nadu, India. We explore and compare the performance of two state-of-the-art self-supervised learning models—**Wav2Vec2.0** and **HuBERT**—to build an efficient ASR system using a custom speech dataset.

---

## 📌 Highlights

- 📦 Custom dataset of **9,837 audio samples** from 11 native speakers
- 🔤 Includes English translations, Badaga transliterations, and speaker metadata
- 🔧 Models used: `Wav2Vec2.0`, `HuBERT` (Transformer-based SSL models)
- 🎯 Evaluation Metric: **Word Error Rate (WER)**
- ✅ Achieved WER of **16.5%** using HuBERT and **16.8%** using Wav2Vec2.0

---

## 🧠 Technologies & Tools

- Python
- PyTorch
- Hugging Face Transformers
- Librosa, NumPy, Pandas
- Jupyter Notebook

---

## 📊 Dataset Summary

| Attribute              | Value              |
|------------------------|--------------------|
| Total Samples          | 9,837              |
| Total Speakers         | 11 (balanced gender)|
| Average Duration       | 2.41 seconds       |
| Average Words per Sample | 5.13            |
| Training Samples       | 6,897              |
| Validation Samples     | 1,470              |
| Test Samples           | 1,470              |


---

## 🔄 Workflow Overview

1. **Data Collection & Annotation**
2. **Preprocessing**: Silence trimming, normalization, tokenization
3. **Model Fine-Tuning**: On custom Badaga speech corpus
4. **Evaluation**: WER & qualitative error analysis
5. **Comparison**: HuBERT vs. Wav2Vec2.0

---

## 📈 Results

| Model       | WER   |
|-------------|--------|
| HuBERT      | **16.5%** |
| Wav2Vec2.0  | 16.8%  |

HuBERT slightly outperformed Wav2Vec2.0 due to its masked prediction and cluster-based learning strategy.

---

## 💡 Future Work

- 🔁 Data augmentation with dialect and speaker diversity
- 🌍 Multilingual transfer learning and model ensembling
- 🧠 Language model integration for improved syntax understanding
- 📱 Real-time ASR deployment on embedded/mobile platforms
- 🔒 Speaker adaptation for privacy and personalization

---

## 👨‍💻 Authors

- [Snega Sri A](mailto:snegasria3@gmail.com)  
- M. Vasista  
- Nandana Gireesh  
- N. Dakshinya  

Department of Artificial Intelligence  
Amrita Vishwa Vidyapeetham, Coimbatore

---

## 📚 References

1. [Baevski et al., "Wav2Vec 2.0", NeurIPS 2020](https://arxiv.org/abs/2006.11477)  
2. [Hsu et al., "HuBERT: Self-Supervised Speech Representation Learning", 2021](https://arxiv.org/abs/2106.07447)  

---


