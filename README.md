# Analysis of Single-Channel Speech Enhancement Methods Using STFT: Spectral Subtraction, Wiener Filtering, and MMSE-STSA

## Overview
This project implements a speech enhancement system in MATLAB using classic frequency-domain noise suppression algorithms in the short-time Fourier transform (STFT) domain.
The system compares three enhancement methods:
- Spectral Subtraction
- Wiener Filtering
- MMSE Short-Time Spectral Amplitude Estimation (MMSE-STSA)

The goal is to improve intelligibility and clarity of speech recordings corrupted by background noise by estimating the noise spectrum, applying frequency-dependent gain functions, and reconstructing an enhanced waveform using inverse STFT.


---


## Motivation
Speech in real environments is often masked by background noise—public transport, crowds, engine noise, or indoor ambience. This reduces clarity and affects communication, recordings, and speech-driven systems.
While deep learning methods (e.g., DCCRN, RNNoise, Conv-TasNet) achieve strong results, they require heavy computation and are less interpretable.

This project focuses on classical DSP approaches that are:

- lightweight
- transparent
- suitable for real-time use


---


## Updates and Progress
- Noise generation using controlled SNR mixing (clean + real airport noise).
- STFT analysis using a 32 ms Hann window with 50% overlap.
- Implemented:
  - Spectral Subtraction with oversubtraction and flooring.
  - Wiener Filtering with decision-directed SNR estimation.
  - MMSE-STSA using stable Bessel-function-based gain computation.
- Developed evaluation tools:
  - Waveform comparisons
  - Spectrogram comparisons
  - Segmental SNR over time
  - Spectral flatness (musical noise indicator)
  - Gain heatmaps and histograms
  - Noise PSD estimation checks
  - α–β parameter sweep for spectral subtraction
  - Residual spectrograms (clean – enhanced)

 
---


## Literature Review Summary
Several foundational studies and follow-up research contributed to the design choices in this project:

- Boll (1979) – introduced spectral subtraction for stationary noise reduction.
- Berouti et al. (1979) – proposed oversubtraction and spectral flooring to reduce musical noise.
- Ephraim & Malah (1984) – developed the MMSE-STSA estimator, widely regarded for achieving smooth and natural enhancement.
- Loizou (2013) – analysed perceptual effects and implementation details of classical noise-suppression algorithms.


---


👤 **Author:** Joshua Chao-Hsu Chen
📘 **Course:** ELEC5305 - Acoustics, Speech, and Signal Processing
🗂️ **GitHub Repo:** https://github.com/JoshuaCHChen/elec5305-project-510656681
