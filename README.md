# ImpliHateVid:A Benchmark Dataset and Two-stage Contrastive Learning Framework for Implicit Hate Speech Detection in Videos

This repository contains the codes used in the implementation of the paper.

# Abstract
The existing research has primarily focused on text and image-based hate speech detection, video-based approaches remain underexplored. In this work, we introduce a novel dataset, ImpliHateVid, specifically curated for implicit hate speech detection in videos. ImpliHateVid consists of 2,009 videos comprising 509 implicit hate videos, 500 explicit hate videos, and 1,000 non-hate videos, making it one of the first large-scale video datasets dedicated to implicit hate detection. We also propose a novel two-stage contrastive learning framework for hate speech detection in videos. In the first stage, we train modality-specific encoders for audio, text, and image using contrastive loss by concatenating features from the three encoders. In the second stage, we train cross-encoders using contrastive learning to refine multimodal representations. Additionally, we incorporate sentiment, emotion, and caption-based features to enhance implicit hate detection. We evaluate our method on two datasets, ImpliHateVid for implicit hate speech detection and another dataset for general hate speech detection in videos, HateMM dataset, demonstrating the effectiveness of the proposed multimodal contrastive learning for hateful content detection in videos and the significance of our dataset.

# Overall Architecture of the Model
We propose a two-stage contrastive learning multimodal framework for detecting hateful content in videos as shown in the figure below. Our approach comprises three key steps: (i) preprocessing to extract audio, text, and visual data; (ii) feature extraction using modality-specific encoders; and (iii) contrastive learning to align representations, culminating in a multimodal classifier.

![Group 258](https://github.com/user-attachments/assets/39361ac4-ff62-4e15-99b1-2024bbcc7c73)

# Overview
Run [Frame Extraction of Videos.ipynb](https://github.com/videohatespeech/Implicit_Video_Hate/blob/main/Codes/Frame%20Extraction%20of%20Videos.ipynb) for extracting frames from the videos.</br>
Run [Audio Extraction from Videos.ipynb](https://github.com/videohatespeech/Implicit_Video_Hate/blob/main/Codes/Audio%20Extraction%20from%20Videos.ipynb) for extracting audio from videos</br>
Run [Text Extraction from Audio.ipynb](https://github.com/videohatespeech/Implicit_Video_Hate/blob/main/Codes/Text%20Extraction%20from%20Audio.ipynb) for extracting transcripts from audio files</br>
Run [Emotion and Sentiment Scores.ipynb](https://github.com/videohatespeech/Implicit_Video_Hate/blob/main/Codes/Emotion%20and%20Sentiment%20Scores.ipynb) for getting emotion and sentiment scores from transcripts</br>
Run [Caption Generation.ipynb](https://github.com/videohatespeech/Implicit_Video_Hate/blob/main/Codes/Caption%20Generation.ipynb) for generating captions from image frames</br>
Run [Extracting ImageBind Features.ipynb](https://github.com/videohatespeech/Implicit_Video_Hate/blob/main/Codes/Extracting%20ImageBind%20Features.ipynb) for getting the ImageBind embeddings of the three modalities</br>
Run [Multistage Contrastive Learning](https://github.com/videohatespeech/Implicit_Video_Hate/blob/main/Codes/Multistage%20Contrastive%20Learning.ipynb) for running the model

# Dataset 

The dataset can be accessed at: [ImpliHateVid Dataset](https://indianinstituteoftechindore-my.sharepoint.com/my?id=%2Fpersonal%2Fphd2101201005%5Fiiti%5Fac%5Fin%2FDocuments%2FImpliHateVid).

| Properties  | Non Hate | Implicit Hate | Explicit Hate |
| ------------- | ------------- | ------------- | ------------- |
| Video count  | 1000 (49.78%)  | 509 (25.36%) | 500 (24.89%) |
| Total length  | 39 hours 26 mins 42 secs  | 18 hours 7 mins 51 secs | 28 hours 58 mins 25 secs |
| Mean video length | 2 mins 22 secs | 2 mins 8 secs | 2 mins 38 secs |
| Total number of frames | 1,42,002 | 65,271 | 79,105 |
| Mean number of frames | 142.002 | 128.23 | 158.21 |
| Mean number of words | 175.404 | 85.166 | 80.326 |
