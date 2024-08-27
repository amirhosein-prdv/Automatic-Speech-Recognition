# Automatic-Speech-Recognition

## Project Overview

This repository contains the final project for the **Machine Learning** course at the [Tehran University of Technology's Faculty of Electrical and Computer Engineering](https://www.ut.ac.ir/en), focused on **Automatic Speech Recognition (ASR)**. The project involves data preprocessing, feature extraction, classification, and clustering models to enhance the accuracy and efficiency of speech recognition systems.

## Table of Contents

- [Introduction](#introduction)
- [Data Processing](#data-processing)
- [Feature Extraction](#feature-extraction)
- [Classification Models](#classification-models)
- [Clustering Models](#clustering-models)
- [Automatic Speech Recognition (ASR)](#automatic-speech-recognition-asr)
- [Results](#results)
- [References](#references)
- [License](#license)

## Introduction

The project aims to develop and compare various machine learning models for speech recognition. It involves detailed data processing techniques and feature extraction methods to improve the performance of ASR systems.

## Data Processing

We applied several data preprocessing techniques to enhance the quality and usability of the audio data:

- **Resampling**: Adjusting the sampling rate of audio signals.
- **Trimming**: Removing unnecessary silence from the start and end of the audio files.
- **Normalization**: Scaling the audio signals to a standard range.
- **Preemphasis**: Amplifying high frequencies to improve signal quality.

## Feature Extraction

Key features were extracted from the audio signals to aid in model training:

- **MFCC**: Mel-frequency cepstral coefficients.
- **Chroma STFT**: Chromagram from a short-time Fourier transform.
- **Spectral Contrast**: Difference in amplitude between peaks and valleys in a sound spectrum.
- **Spectral Centroid**: Represents the "center of mass" of the sound spectrum.

## Classification Models

We experimented with various classification models to categorize the audio data:

- **Support Vector Machine (SVM)**
- **Random Forest (RF)**

Improvements were made to these models by fine-tuning their parameters and comparing their performance using accuracy, confusion matrices, and ROC curves.
Also we used Dimension reduction algorithms like **Principal Component Analysis (PCA)** and **Linear Discremenant Analysis (LDA)** to use best features.
## Clustering Models

In addition to classification, clustering models were used to group similar audio features:

- **K-Means Clustering**
- **Hierarchical Clustering**

## Automatic Speech Recognition (ASR)

The Automatic Speech Recognition (ASR) component is the core of this project. ASR is the process of converting spoken language into text, and it plays a crucial role in various applications, such as virtual assistants, transcription services, and voice-controlled interfaces.


![image](https://github.com/user-attachments/assets/2d516ead-baa2-4c90-964b-1f55bae1c74b)


### Approach

Our approach leverages **Wav2Vec**, a state-of-the-art model for speech processing, combined with **Transformer** architectures to enhance accuracy and efficiency. Here's a breakdown of the steps involved:

1. **Wav2Vec Model**:
   - The Wav2Vec model is pre-trained on large datasets of unlabeled audio, learning to predict masked parts of the waveform from the surrounding context.
   - After pre-training, the model is fine-tuned on a labeled dataset, where the objective is to classify phonemes, words, or other linguistic units.

2. **Transformer Architecture**:
   - We utilize the Transformer model, known for its success in natural language processing tasks, to handle the sequential data of speech.
   - The Transformer's attention mechanism allows it to focus on different parts of the input sequence, improving the recognition of complex speech patterns.

3. **Fine-Tuning**:
   - Fine-tuning involves adjusting the Wav2Vec model parameters on our specific dataset, optimizing for speech-to-text accuracy.
   - The training process focuses on minimizing loss and improving the model's ability to generalize to different speakers, accents, and noise conditions.

### Challenges Addressed

- **Noise Reduction**: Dealing with background noise in audio recordings.
- **Speaker Variability**: Handling different accents, pitches, and speaking speeds.
- **Real-Time Processing**: Ensuring the ASR system works efficiently for real-time applications.

### Evaluation

The ASR system's performance is evaluated using metrics like Word Error Rate (WER), accuracy, and computational efficiency. The results demonstrate the effectiveness of the Wav2Vec and Transformer-based approach in achieving high accuracy in diverse conditions.

## Results

The project results include a comprehensive comparison of the models' performance, including their accuracy and computational efficiency. The best-performing models were identified, and suggestions for further improvements were discussed. For more information about results, check report file.

## References

[1] Raahul, A., Sapthagiri, R., Pankaj, K., & Vijayarajan, V. (2017). Voice based gender
classification using machine learning. In IOP Conference Series: Materials Science and
Engineering (Vol. 263, p. 042083). IOP Publishing. https://doi.org/10.1088/1757-
899x/263/4/042083

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
