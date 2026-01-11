# 🐏 Animal Sound Identifier
This repository contains a Jupyter notebook that serves as a practical example of how to utilize PyTorch Lightning for a multiclass audio classification task. In this instance, we have selected a subset of [YashNita's Animal Sound Dataset](https://github.com/YashNita/Animal-Sound-Dataset), focusing on five specific animal classes: chicken, cow, donkey, frog, and sheep. Each sound file is labeled with exactly one class. To extract features from the audio data, we employ the [Librosa](https://librosa.org/doc/latest/index.html) library, which is well-regarded for its robust audio analysis capabilities. The model architecture contains two convolutional layers, each followed by a max pooling layer, leading into a fully connected layer designed to enhance classification performance. However, it is important to note that the model's accuracy is currently not satisfactory, indicating ample opportunity for improvement.

<img src="https://raw.githubusercontent.com/bshtmichielsen/animal_sound_identifier/refs/heads/main/BANNER.jpg" />

*Image by Stable Diffusion: a machine that can classify animal sounds*

This notebook is intentionally designed as a foundational starting point and does not strictly adhere to established best practices as it is meant as a learning opportunity. This repo belongs to a five part course:&nbsp;&nbsp;&nbsp; 🏠&nbsp;[House&nbsp;Price&nbsp;Predictor](https://github.com/bshtmichielsen/house_price_predictor)&nbsp;&nbsp;&nbsp; 🐏&nbsp;[Animal&nbsp;Sound&nbsp;Identifier](https://github.com/bshtmichielsen/animal_sound_identifier)&nbsp; &nbsp;👗&nbsp;[Clothing&nbsp;Sorter](https://github.com/bshtmichielsen/clothing_sorter)&nbsp;&nbsp;&nbsp; 🍎&nbsp;[Fruit&nbsp;Detector](https://github.com/bshtmichielsen/fruit_detector)&nbsp;&nbsp;&nbsp; 💬&nbsp;[Expert&nbsp;Chat](https://github.com/bshtmichielsen/expert_chat)&nbsp; Feel free to learn from the other parts too!

## 📚 Preparation
Please ensure that you are familiar with the following aspects in order to successfully work with this repo and notebook.
 - You can explain the difference between [classification and regression](https://www.geeksforgeeks.org/machine-learning/ml-classification-vs-regression/) problems.
 - You know what a class is and how some problems can be [multiclass or multilabel](https://www.geeksforgeeks.org/machine-learning/multiclass-classification-vs-multi-label-classification/).
 - You understand the general idea of [feature extraction](https://www.geeksforgeeks.org/machine-learning/what-is-feature-extraction/).


## 🎯 Learning opportunities
The following aspects of machine learning are part of this example:
- Working with data files, in this case audio file
- Feature extraction using a specialistic library
- Neural Network building using layers
- Accuracy, Precision, Recall
- Confidence scores

## 🤔 Considerations for improvement
This notebook is an example on how to get started, it is open for improvements and enhancements. Feel free to clone my work and use it to study and learn. Things to consider if you want to improve this work:
- Currently only 13 MFCC features are extracted from librosa, quite likely additional features may be interesting to try or perhaps add.
- When the model gives a correct prediction with a high confidence score, the model performs better than when it gives a correct prediction but with a low confidence score. Alternatively, when the model predicts wrongly with a high confidence score, this feels more wrong than when it does so with a low confidence score. We currently have no metric to measure this difference, as we only look at correct/wrong. Could you devise a metric for this?
- There is no evaluation on whether the model is overfitted, it may very well be.
- more?

## ⭐ Citation & Star
If you use my work please cite and star ⭐ this repo. Thanks!
> Michielsen, Bas S.H.T. (2025) "Animal Sound Identifier" GitHub: https://github.com/bshtmichielsen/animal_sound_identifier