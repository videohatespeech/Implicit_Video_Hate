# ImpliHateVid:A Benchmark Dataset and Two-stage Contrastive Learning Framework for Implicit Hate Speech Detection in Videos
Published in ACL-2025, **[Link](https://aclanthology.org/2025.acl-long.842/)**  

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

| Properties  | Non Hate | Implicit Hate | Explicit Hate |
| ------------- | ------------- | ------------- | ------------- |
| Video count  | 1000 (49.78%)  | 509 (25.36%) | 500 (24.89%) |
| Total length  | 39 hours 26 mins 42 secs  | 18 hours 7 mins 51 secs | 28 hours 58 mins 25 secs |
| Mean video length | 2 mins 22 secs | 2 mins 8 secs | 2 mins 38 secs |
| Total number of frames | 1,42,002 | 65,271 | 79,105 |
| Mean number of frames | 142.002 | 128.23 | 158.21 |
| Mean number of words | 175.404 | 85.166 | 80.326 |

# 📦 Dataset Access

Access to the dataset is restricted to academic and research purposes only. Please ensure compliance with the following terms before requesting access.

---

## ✅ Requirements for Access

### 🔒 Non-Commercial Use
- The dataset is **strictly for academic research** and **non-commercial** use.
- **Commercial use**, whether direct or indirect, is **prohibited**.
- You may not use the dataset to develop, train, or market commercial products or services.

### 🚫 No Redistribution
- **Redistribution is not allowed**. Do not share the dataset, in part or in full, on:
  - Public or private repositories
  - Online platforms
  - Social media or forums
- You must store the dataset in **secure environments** and prevent access by unauthorized individuals.

### 📜 Compliance with Platform Policies
- The dataset is derived from publicly available **BitChute and Odysee** data.
- You must comply with the BitChute and Odysee Developer Agreement and Policy.
- Pay special attention to data usage, privacy, and **content redistribution rules**.

### 🎓 Academic Integrity
- The dataset must be used only for **legitimate academic research**.
- Ensure your usage aligns with institutional **ethical standards**, especially regarding privacy and responsible AI practices.

---

## 📬 Access Request Procedure

1. **Use your institutional email** for all communications.  
   > Requests from personal email addresses may not be ignored.

2. Fill out the **[Dataset Agreement Form](https://docs.google.com/document/d/1Cb_f-xhOobgpnn_u2lOB6_m1lCHlDNCt/edit)**.

3. Upload the signed consent in the **[Dataset Request Form](https://docs.google.com/forms/d/1UTItZLZXqZ7h_dT73wBk8YDkMRtKItUBYV8zznsiRKk/edit)** along with your details.

4. Once reviewed and approved, you will receive an email with **dataset download instructions**.

# 📄 Related Paper

You can read more about the dataset and its applications in the accompanying paper:

**[ImpliHateVid: A Benchmark Dataset and Two-stage Contrastive Learning Framework for Implicit Hate Speech Detection in Videos](https://aclanthology.org/2025.acl-long.842/)**  

# 📖 Citation

If you use this dataset in your research, please cite our work as follows:

```bibtex
@inproceedings{rehman-etal-2025-implihatevid,
    title = "{I}mpli{H}ate{V}id: A Benchmark Dataset and Two-stage Contrastive Learning Framework for Implicit Hate Speech Detection in Videos",
    author = "Rehman, Mohammad Zia Ur  and
      Bhatnagar, Anukriti  and
      Kabde, Omkar  and
      Bansal, Shubhi  and
      Kumar, Dr. Nagendra",
    editor = "Che, Wanxiang  and
      Nabende, Joyce  and
      Shutova, Ekaterina  and
      Pilehvar, Mohammad Taher",
    booktitle = "Proceedings of the 63rd Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers)",
    month = jul,
    year = "2025",
    address = "Vienna, Austria",
    publisher = "Association for Computational Linguistics",
    url = "https://aclanthology.org/2025.acl-long.842/",
    pages = "17209--17221",
    ISBN = "979-8-89176-251-0"
}
}
