<h1 align="center">
<br>
  <img src="wav2vec2.png" alt="Diagram" >
  <br>
    <br>
  Wav2Vec2 Fine-Tuning for ASR
  <br>
</h1>
 
### Autor: Salma OUARDI

This repository contains an implementation of fine-tuning the Wav2Vec2 model for Automatic Speech Recognition (ASR). Wav2Vec2 is a pretrained model that has shown competitive results to state-of-the-art ASR systems with as little as 10 minutes of labeled data. 

In this project, we fine-tune Wav2Vec2 on speech datasets for Spanish and Finnish, aiming to develop a model that performs well on low-resource languages. We investigate whether an English pretrained model performs better than a multilingual pretrained model for Finnish and Spanish ASR.

## Project Steps

1. Connect to the Hugging Face hub to save our checkpoints.
2. Mount Google Drive to save the trainer's logs.
3. Set up the Kaggle API.
4. Load and preprocess the [CSS10] dataset: A Collection of Single Speaker Speech Datasets for 10 Languages.
5. Configure the Wav2Vec2CTCTokenizer and Wav2Vec2FeatureExtractor.
6. Fine-tune and train the model, then evaluate it on the test data using the Word Error Rate (WER) metric.
7. Save the model and processor (tokenizer + feature extractor) in the Hugging Face hub and the logs in Google Drive.

## Results

The fine-tuned model achieved a Word Error Rate (WER) of less than 5% on the test sets. The specific results were:

- Spanish WER: 0.165
- Finnish WER: 0.376

These results demonstrate the effectiveness of the fine-tuning approach on Wav2Vec2 for ASR, even for low-resource languages.

## Usage

To use this project, clone the repository to your local machine and run the Jupyter notebook. Make sure to set up the Hugging Face and Kaggle APIs, and mount your Google Drive if you want to save the logs.

## Future Work

Future updates will include fine-tuning Wav2Vec2 on more low-resource languages and comparing the performance of different pretrained models.

## Credits

This project was a collaborative effort. Many thanks to [Hugging Face](https://huggingface.co/) for providing the Wav2Vec2 model and the platform to share our work.
Many thanks to my classmate [Romain Mussard](https://github.com/RomainMsrd) for his valuable contributions.
