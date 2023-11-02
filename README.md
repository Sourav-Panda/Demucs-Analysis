# Demucs-Analysis
Analysis of Demucs for Music Source Separation on Waveform Domain. 
## Overview
Music source separation refers to the task of separating individual instrument sources (vocals, drums, bass, etc) from a mixed music recording. Recent deep learning models like Demucs have shown promising results by operating directly on the waveform rather than the spectrogram. In this dissertation, I investigate using the Demucs model for music source separation and compare its performance to other state-of-the-art waveform separation models like ConvTasnet. I also analyze how well Demucs generalizes to different music genres and how robust it is to noisy input mixtures.

models: I have used the Demucs v2 for my analysis
data: contains downloaded datasets like MUSDB18 and a custom Bollywood dataset, curated by me.
experiments: notebooks and scripts to run experiments and visualize results
## Experiments
The key experiments covered in this dissertation are:

- Training Demucs on the MUSDB dataset and evaluating source separation performance
- Testing Demucs generalization on a Bollywood music dataset with new instruments/style
- Analyzing Demucs performance on noisy mixtures with additive white Gaussian noise
- Comparing Demucs with other waveform models like ConvTasnet
