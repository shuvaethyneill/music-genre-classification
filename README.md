# music-genre-classification

---
> **Preamble:** This notebook was adapted from an Introduction to Machine Learning course assignment. It is intended to demonstrate an understanding of classification models and exploration of concepts in machine learning.
---

> **Goal:** To develop a music genre detection machine learning model using audio files.

> **Objective:**: Use the GTZAN dataset to create a classifier that can classify what music genre is playing! 🎷🎸🎹🎺
Develop 2 models: 
- 1. A custom-trained model for this task
- 2. A ‘baseline solution’ that uses a pre-trained classifier and fine-tuned it on the musical genre classification task using transfer learning

> **Instructions:** The entire full notebook should run in under 40 minutes on T4 GPU. The solutions for this notebook are self-contained. This notebook was intended to be executed and tested on Google Colab. Using the commands: `runtime → run all`.

> **Dataset:** GTZAN Dataset.

Download from source: https://www.kaggle.com/datasets/andradaolteanu/gtzan-dataset-music-genre-classification?resource=download

Placed under `My Drive` in the Google Drive directory and renamed as `GTZAN Genre Collection.zip`

Music. Experts have been trying for a long time to understand sound and what differentiates one song from another. How to visualize sound. What makes a tone different from another? This data hopefully can allow doing just that.

- *genres original* - A collection of 10 genres with 100 audio files each, all having a length of 30 seconds (the famous GTZAN dataset, the MNIST of sounds)
- *images original* - A visual representation for each audio file. One way to classify data is through neural networks. Because NNs (like CNN, what we will be using today) usually take in some sort of image representation, the audio files were converted to Mel Spectrograms to make this possible.
- *2 CSV files* - Containing features of the audio files.

> **Runtime Tips:** Select `Runtime -> Change Runtime Type` under `Hardware accelerator` and click on `CPU` or `T4 GPU`.

## Distribution of Data
![distribution](https://github.com/shuvaethyneill/music-genre-classification/assets/23216104/862e30e4-0e48-4b61-ad5b-44c9fd6b8d33)

## Performance of Custom-Trained Model
![custom](https://github.com/shuvaethyneill/music-genre-classification/assets/23216104/57aa7d59-46b4-48b1-b2e3-d837123162c2)
