# Capuchin Bird Call Classification

## Overview

In this project, I built a deep learning pipeline to detect and count capuchin bird calls in long rainforest audio recordings. I used TensorFlow to convert short audio clips into spectrograms, trained a CNN classifier, and then scanned full-length recordings using a sliding window approach to estimate bird call density.

---

## Summary

- I started by converting `.wav` and `.mp3` files to mono 16kHz waveforms.
- Then I padded and transformed each clip into a spectrogram using Short-Time Fourier Transform (STFT).
- I trained a convolutional neural network to classify clips as either Capuchin or not.
- I applied this model across 3-minute forest recordings in 3-second segments.
- Finally, I grouped consecutive detections and exported the call counts to a CSV.

---

## Technologies used

- **TensorFlow 2.4.1** – for building and training the neural network  
- **TensorFlow-IO** – for audio decoding and resampling  
- **Matplotlib** – for visualizing waveforms and spectrograms  

---

## Impact

This project shows how machine learning can automate wildlife monitoring by identifying animal calls in dense, real-world audio. It mimics real applications like voice detection in Siri or Alexa and can be adapted for conservation work, biodiversity tracking, and acoustic research in the field.

## Why I built this

I wanted to explore how deep learning can be applied to audio, especially in real-world, noisy environments. Most of my previous work focused on computer vision, so this was a chance to learn a new modality: sound! This project helped me better understand signal processing, spectrograms, and how to structure machine learning pipelines for audio classification.
