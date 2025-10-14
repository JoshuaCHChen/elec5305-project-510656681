# Real-Time speech Enhancement Using FFT-Based Noise Suppression

## Overview
This project implements a speech enhancement system in **MATLAB** using **spectral subtraction** in the **short-time Fourier transform (STFT) domain**.  
The goal is to improve intelligibility of speech recordings corrupted by background noise by estimating and subtracting the noise spectrum, then reconstructing the enhanced waveform.

## Motivation
Background noise reduces clarity in everyday communication, especially in mobile calls, video conferencing, and hearing aids. While deep learning solutions exist, they are computationally expensive and less transparent.  
This project demonstrates an interpretable approach that extends classical DSP methods taught in the course, showing how they can be applied to real-world audio problems.

---

## Updates and Progress
- Implemented an initial MATLAB prototype performing:
  - Noise simulation using `awgn()`.
  - STFT analysis of clean and noisy speech signals.
  - Spectral subtraction with noise floor limiting.
  - Inverse STFT for waveform reconstruction.
- Spectrogram comparisons confirm reduced high-frequency noise components after processing.
- Current focus:

## Literature Review Summary
Recent studies show hybrid or adaptive versions of spectral subtraction can outperform static methods.  
Key findings:
- Boll (1979) introduced baseline spectral subtraction for stationary noise.
- Berouti et al. (1979) proposed oversubtraction and spectral flooring to reduce distortion.
- Loizou (2013) and Kamath & Loizou (2002) discuss real-time implementations and perceptual weighting.
- Deep learning models (e.g., RNNoise, DCCRN) achieve superior results but are computationally heavy—this project focuses on efficient classical DSP methods.


---

👤 **Author:** Joshua Chao-Hsu Chen
📘 **Course:** ELEC5305 - Acoustics, Speech, and Signal Processing
🗂️ **GitHub Repo:** https://github.com/JoshuaCHChen/elec5305-project-510656681
