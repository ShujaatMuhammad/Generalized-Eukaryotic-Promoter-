# Species-aware Eukaryotic Promoter Prediction and Strong/Weak Promoter Classification

This repository contains the implementation of a two-stage computational framework for generalized eukaryotic promoter prediction and species-aware promoter strength classification.

The framework first predicts whether a query DNA sequence is a promoter or non-promoter using multi-species promoter data. In the second stage, promoter strength is classified as strong or weak using transcriptional activity labels derived from FANTOM5 CAGE data. The project also includes explainable AI analysis using attention-based motif discovery and SHAP-based nucleotide-level attribution.

---

## Overview

Promoters are key regulatory DNA elements that define transcription initiation and influence gene-expression output. Although many promoter prediction models have been developed, most existing tools are limited to prokaryotic genomes, single-species prediction, or binary promoter/non-promoter classification.

This project addresses these limitations by developing:

1. A generalized eukaryotic promoter/non-promoter prediction model trained on promoter sequences from multiple eukaryotic species.
2. A promoter strength classification framework that predicts strong versus weak promoters using CAGE-derived transcriptional activity.
3. A species-aware interpretation strategy to analyze motif-switching behavior across species.
4. Explainable AI modules using attention scores and SHAP values to identify important promoter regions, nucleotides, and motifs.

---

## Main Features

- Multi-species eukaryotic promoter benchmark construction
- GC-matched non-promoter dataset generation
- Multiple DNA feature encoding schemes
- Classical machine learning and deep learning model comparison
- CNN–BiLSTM attention model for promoter/non-promoter prediction
- CNN-based strong/weak promoter classification
- FANTOM5 CAGE-derived promoter strength labeling
- Attention-based motif analysis
- SHAP-based nucleotide and position-level interpretation
- Motif-switching analysis across species

---

## Dataset Description

### Promoter Dataset

Experimentally validated promoter sequences were collected from EPDnew across 16 eukaryotic species. Each promoter sequence was extracted as a fixed-length 300 bp window relative to the transcription start site:

```text
−249 bp upstream to +50 bp downstream of TSS
