# 🧬 Species-aware Eukaryotic Promoter Prediction  
### A Two-stage Framework for Generalized Promoter Recognition and Strong/Weak Promoter Classification

<p align="center">
  <img src="docs/graphical_abstract.png" width="850"/>
</p>

<p align="center">
  <b>Multi-species promoter prediction • Promoter strength classification • CNN–BiLSTM attention • SHAP explainability</b>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.8%2B-blue"/>
  <img src="https://img.shields.io/badge/PyTorch-Deep%20Learning-red"/>
  <img src="https://img.shields.io/badge/SHAP-XAI-purple"/>
  <img src="https://img.shields.io/badge/Bioinformatics-Promoter%20Prediction-green"/>
  <img src="https://img.shields.io/badge/License-MIT-lightgrey"/>
</p>

---

## 📌 Overview

This repository provides the implementation of a **two-stage species-aware framework** for generalized eukaryotic promoter analysis.

The first stage predicts whether a query DNA sequence is a **promoter** or **non-promoter** using multi-species promoter data from **EPDnew**. The second stage classifies validated promoters as **strong** or **weak** using **FANTOM5 CAGE-derived transcriptional activity values**.

The framework also includes model interpretation using **attention-based motif analysis** and **SHAP-based nucleotide-level attribution**.

---

## ✨ Key Contributions

| Feature | Description |
|---|---|
| 🧬 Multi-species promoter prediction | Promoter/non-promoter classification across diverse eukaryotic species |
| 🧪 GC-matched negative dataset | Species-wise non-promoter sequences with comparable GC-content |
| 🤖 Deep learning model | CNN–BiLSTM attention model for promoter prediction |
| 📊 Promoter strength classification | Strong/weak promoter labels using FANTOM5 CAGE activity |
| 🔍 Explainable AI | Attention motifs and SHAP-based nucleotide attribution |
| 🌍 Species-aware interpretation | Motif-switching analysis across species |

---

## 🧠 Framework Summary

```text
EPDnew promoters + species-matched non-promoters
                    ↓
        Multi-species benchmark dataset
                    ↓
       Feature encoding and model comparison
                    ↓
          CNN–BiLSTM attention model
                    ↓
       Promoter vs non-promoter prediction
                    ↓
 Attention-based motif analysis + SHAP interpretation
                    ↓
 FANTOM5 CAGE-based strong/weak promoter classification
                    ↓
      Species-aware motif-switching analysis
