Lung Disease Detection
This repository contains a deep learning model designed for classifying respiratory sounds into various disease categories. The model leverages a combination of Convolutional Neural Networks (CNNs) and Recurrent Neural Networks (RNNs) to extract meaningful features from audio recordings of respiratory sounds.

Dataset
The Respiratory Sound Database serves as the foundation for this project. This dataset includes audio recordings of respiratory sounds collected from patients diagnosed with various respiratory diseases.

Model Architecture
The model integrates three feature extraction methods and combines their outputs for enhanced classification performance:

MFCC Model:

Extracts Mel-Frequency Cepstral Coefficients (MFCCs) from the audio recordings.
Uses a CNN for classifying the features.
CSTFT Model:

Extracts Constant-Q Transform (CQT) features from the audio recordings.
Utilizes a CNN for feature classification.
MSPEC Model:

Extracts Mel-Spectrogram features from the audio recordings.
Employs a CNN for classification.
The outputs of these three models are concatenated and passed into a fully connected neural network to generate the final classification results.

Training
Dataset Size:

Total: 6,898 audio recordings
Training Set: 5,173 recordings
Testing Set: 1,725 recordings
Training Parameters:

Epochs: 53
Batch Size: 32
Results
The model achieved an accuracy of 90.49% on the test set, demonstrating its effectiveness in classifying respiratory diseases from audio recordings.
