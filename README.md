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
I have done all my experiments from the Mac environment using the university Hex servers.

## The following programming languages and packages will be utilized in this study:
1.	Python 3.7 or above
2.	Numpy 1.22.1
3.	Matplotlib for data vizualisation.
4.	Pytorch 1.11.0 
5.	Cuda tool kit 11.3
6.	Librosa 0.7.2
7.	ffmpeg 0.2.0
8.	torchaudio 0.11.0+cu113
9.	tqdm 4.36.0
10.	diffq 0.2.0
11.	Julius 0.2.3
12.	Lameenc 1.2.1
13.	Musdb 0.3.1
14.	Museval 0.4.0
15.	Nussl 1.1.9
16.	Pandas 1.4.2
17.	Scipy 1.7.3
18.	Musdb 0.3.1
19.	Museval 0.4.0
20.	mir-eval 0.7
21.	ffmpeg-python 0.2.0
22.	scaper 1.6.4
23.	stempeg 0.2.3
24.	tqdm 4.36.0
25.	torchaudio 0.11.0+cu113
26.	torchvision 0.12.0+cu113
27.	SoundFile 0.10.3.post1
28.	soundstretch


•	I have used SSH from mac terminal to communicate with hex university server.

•	To train the model: in the root demucs folder run the command: python3 -m demucs -b 4  --musdb [musdb path] --epochs 30 --is_wav [for wav data base/ raw for raw data] -d [gpu number]
•	To save the model woth best validation state:  python3 -m demucs -b 4  --musdb [musdb path] --epochs 30 --is_wav [for wav data base/ raw for raw data] -d [gpu number] --save_model
•	To fine tune the pretrained model: python3 -m demucs -b 4  --musdb musdb [musdb path --epochs [number of epochs] --is_wav [for wav data base/ raw for raw data]  -d [gpu number] --init [model name]

Musdb data set can be downloaded from: https://sigsep.github.io/datasets/musdb.html
![image](https://github.com/Sourav-Panda/Demucs-Analysis/assets/95696755/4e291e95-1dd0-4db1-b714-991b5538c54e)
