# Myanmar Speech-Activated Voic-Based Chatbot Campus Navigation - Keyword Spotting Models

This repository contains three trained deep learning models for keyword spotting in a Myanmar language campus navigation chatbot. The models were obtained from 3-fold stratified cross-validation and are designed to classify 7 keywords from short audio clips.

## Model Details

- Input: Log Mel spectrogram images of size 224 x 224 pixels
- Model architecture: Transfer learning with ResNet50 pretrained on ImageNet, fine-tuned for audio classification
- Dataset: Limited dataset (~545 samples per keyword), augmented using noise addition, pitch shifting, and tempo changing
- Techniques: Class weighting and stratified K-Fold cross-validation used to handle imbalanced data and improve generalization
- Accuracy: Achieved 97% accuracy on unseen test data
- Deployment: Models are deployed offline on Raspberry Pi for real-time keyword spotting

## Files

- `model_fold_1.h5`
- `model_fold_2.h5`
- `model_fold_3.h5`

(Note: Due to file size limitations, trained models are hosted on Google Drive. Please use the links below to download.)

## Download Links

- [Model Fold 1](https://drive.google.com/file/d/1aVQJ2hw11HBnAFk8SSIPp5Gyntji_3DZ/view?usp=drive_link)  
- [Model Fold 2](https://drive.google.com/file/d/1RX_531-mWNfif-JulfNnmoF9BnM8V_1I/view?usp=drive_link)  
- [Model Fold 3](https://drive.google.com/file/d/1-UA9FHmjygu-09PVVEMBobgPMxvOunMD/view?usp=drive_link)  

## Usage

These models can be integrated into a real-time keyword spotting system running on embedded devices like Raspberry Pi to assist with voice-based campus navigation in Myanmar Language.

## Technologies Used

- Python  
- TensorFlow  
- Librosa  
- Scikit-learn  
- Google Colab

---

For more information, please contact [yeemonaungstu@gmail].
