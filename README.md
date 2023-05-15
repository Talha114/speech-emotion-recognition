# Project Title

Speech Emotions Recognition (SER)

## Description

In this project, we built a classifier that can determine the emotions concealed in speech signals. We used a dataset of Urdu speech containing emotional utterances from talk shows, with four basic emotions: Angry, Happy, Neutral, and Sad. We extracted three prominent categories of features from the audio files: prosodic features, spectral or vocal tract features, and excitation source features. We then used a support vector machine (SVM) classifier to predict the emotion from the audio features. Additionally, we plotted a scatterplot of the average features of each audio file, with the first half of the features on the x-axis and the second half of the features on the y-axis, colored by the emotion class.

## Getting Started

### Dependencies

* librosa
* numpy
* pandas
* sklearn
* matplotlib

### Installing

You can install the required packages using pip:

```
pip install librosa numpy pandas sklearn matplotlib
```

### Dataset
The dataset for this project contains emotional utterances of Urdu speech gathered from Urdu talk shows. It contains utterances of four basic emotions: Angry, Happy, Neutral, and Sad. There are 38 speakers (27 male and 11 female).
The dataset is already split into training and test sets and provided as separate train and test folders.

### Executing program

* Load the data source for the project.
* Extract the features from the provided audio files.
* Train a model that is able to classify between Angry, Happy, Neutral, & Sad.
* Evaluate the model to check the accuracy of the model.
* Take one audio Test > Sad > SM25_F34_S084.wav and pass it through your model and output the predicted emotion.

## Project Tasks

1. Load the dataset and extract the features from the audio files.
2. Select the classification model and train the model using the extracted features.
3. Evaluate the model to check its accuracy.
4. Take one audio file from the test set and pass it through the model to predict the emotion.
5. Generate a scatterplot to visualize the relationship between the features and emotions.

### Feature Extraction

The following features will be used for classification:

* Mel-frequency cepstral coefficients (MFCC)
* Chroma feature
* Spectral contrast
* Tonnetz

### Model Selection

Support vector machine (SVM) classifier will be used for this project. The linear kernel will be used as the data is expected to be linearly separable.

### Scatterplot

The features for each audio file will be divided into two halves, and the average of the first half and second half will be taken separately for each audio file. A scatterplot will be generated with the first half of the features on the x-axis and the second half of the features on the y-axis. The color of each audio file on the scatterplot will be based on the class to which it belongs.

![19I-1681](https://user-images.githubusercontent.com/88310782/229387074-de0b63a3-a328-4138-a6e5-09965186af94.png)

### Accuracy

The accuracy of the model will be calculated using the `accuracy_score` function from scikit-learn.

## Authors

* OpenAI (model)
* Maryam Baig (implementation)

## Version History

* 1.0
    * Initial Release

## License

This project is licensed under the MIT License - see the [LICENSE.md](https://github.com/MaryamBaig/Speech-Emotions-Recognition/blob/main/LICENSE) file for details.

## Acknowledgments

* This project is inspired by the Speech Emotion Recognition challenge on Kaggle.
