# Gender-and-Age-classification-from-Audio-Files

The code for classifying age and gender using machine learning from audio samples is available in this repository. The IPYNB notebook contains all of the code.

## Data Description
Common Voice is the name of the dataset. A corpus of speech data called Common Voice is read by users on the Common Voice website (http://voice.mozilla.org/), and it is based on text from many public domain sources, including user-submitted blog posts, antiquated books, films, and other public speech corpora. Its main objective is to make it possible for ASR (automatic speech recognition) systems to be trained and tested.

## Data Pre-Processing and Feature Extraction
First, the data is cleaned to remove any NaN values. Then, using the Librosa library, I utilised feature engineering to extract the spectral centroid, spectral bandwidth, and spectral rolloff. The MFCC feature extraction approach was then used to extract more features. The windowing of the signal, application of the DFT, calculation of the magnitude's log, warping of the frequencies on a Mel scale, and application of the inverse DCT are the main steps in the MFCC feature extraction technique.

## Models
Both the gender and age classifications were trained using the random forest classifier. A large number of decision trees are built during the training phase of the random forests or random decision forests ensemble learning approach, which is used for classification, regression, and other tasks.

## Results
1. The Gender Classification achieved the accuracy of 85% and F1 score of 91%
2. The Age Classification achieved the accuracy of 43% and F1 score of 39% which is significantly low. This accuracy can be improved by introducing deep learning models.
