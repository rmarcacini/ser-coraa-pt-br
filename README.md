# Emotion Recognition from Brazilian Portuguese Informal Spontaneous Speech

Here, we present the Brazilian Portuguese Speech Emotion Recognition Task. This task aims to motivate research for SER in our community, mainly to discuss theoretical and practical aspects of Speech Emotion Recognition, pre-processing and feature extraction, and machine learning models for Brazilian Portuguese.

We provide a dataset called CORAA version 6 composed of approximately 50 minutes of audio segments labeled in three classes: neutral, non-neutral female, and non-neutral male. While the neutral class represents audio segments with no well-defined emotional state, the non-neutral classes represent segments associated with one of the primary emotional states in the speaker's speech. This dataset was built from the C-ORAL-BRASIL I corpus (Raso and Mello, 2012).

The available corpus consists of audio segments representing Brazilian Portuguese informal spontaneous speech. The non-neutral emotion class was labeled considering paralinguistic elements (laughing, crying, etc). Participants can use pre-trained models and external data, as long as the original C-ORAL-BRASIL corpus (or variants) is not used for model training.

In this task, participants must train their own models using acoustic audio features. A training set is available. The models trained by the participants will be evaluated in a test set, which will be made publicly available after the challenge.

### Baselines

We present two simple baselines as examples of pre-processing audio segments for feature extraction and model training for emotion recognition.

The first baseline uses a set of prosodic audio features for emotion classification.

* [Pre-processing (Prosodic Features)](https://drive.google.com/file/d/1g9IBNqqPn4WpFTGvoSYm2h7UUAzJSc_q/view?usp=sharing)
* [Model Training (Prosodic Features)](https://drive.google.com/file/d/1hdBMPrfk0-k0RxikBUs113RvNeI3o7j-/view?usp=sharing)
* [Output files and examples](https://drive.google.com/drive/folders/1_jrqArRsNmBD2W4FWGoqNNNJDA7yVjUF?usp=sharing)

In the second baseline, we use the Wav2Vec model to extract features (i.e. embeddings) from the audio segments. These features can be used for training a speech emotion recognition classifier.

* [Pre-processing (Wav2Vec Features)](https://drive.google.com/file/d/1N-QgjCax881LLH1bmsPJyLz707iO8KRc/view?usp=sharing)
* [Model Training (Wav2Vec Features)](https://drive.google.com/file/d/1kausjiMFEM5h1sJQ8CxFmRpnZKQL5-Mc/view?usp=sharing)
* [Output files and examples](https://drive.google.com/drive/folders/1FGdwoaG6ERYVaisMp10TpllxG4Jjsv3o?usp=sharing)

### Evaluation: 

Each participant can submit up to three models. The Macro F1 Score measure will be used to evaluate the models.