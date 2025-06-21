# Speech-to-Text using Traditional ML (HMM + GMM)

This project demonstrates a basic speech recognition system using traditional machine learning techniques — Hidden Markov Models (HMM) and Gaussian Mixture Models (GMM). It classifies spoken words from audio recordings using feature extraction methods like MFCC, delta, and delta² features.

## Problem Statement

To develop a basic speech recognition system that can classify spoken words using classical machine learning models — HMM and GMM — without using any neural networks or pre-trained models.

## Dataset

I used the **Google Speech Commands Dataset** by Google AI.

- **Link to dataset:** [https://www.tensorflow.org/datasets/catalog/speech_commands](https://www.tensorflow.org/datasets/catalog/speech_commands)
- 35+ spoken words
- ~2000 samples per word
- 1-second 16kHz mono WAV files
- Includes background noise folder

> **Note**: Due to dataset size, I have not uploaded it. Please download it manually from the link above.
> **Note**: Due to dataset size, i have not uploaded the feature extracted file but if you run the code it will generate the extracted feature file (.pkl).

## Models Used

### Hidden Markov Model (HMM)
- Suitable for sequence modeling like speech
- 7 hidden states used (can be change)
- Trained with Gaussian emissions

### Gaussian Mixture Model (GMM)
- Models probability distribution of audio features
- Does not account for sequence/time
- One GMM per word, with 7 components

## Tools and Libraries
- Python
- NumPy, Librosa, scipy
- Scikit-learn, HMMlearn
- SoundDevice (for live mic input)
- Matplotlib

## Live Prediction
Record live audio using your microphone and classify the spoken word using both HMM and GMM models.

## 🗃 Files Included
- `speech-to-text_traditional_method.ipynb`: Complete notebook with training, testing, and live prediction
- `requirements.txt`: Python dependencies
- `LICENSE`: MIT License
- `README.md`: This file
- `Trained models` - Both HMM and GMM model that I created and used for predictions

## License
This project is licensed under the MIT License.
