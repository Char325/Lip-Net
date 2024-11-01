# Lip Net
Lip Net is a Machine Learning + Computer Vision project designed to analyze and interpret lip movements for various applications such as silent speech recognition, lip reading, and more.
# Introduction
## Overview
Lip Net is an advanced machine learning and computer vision project designed to analyze and interpret lip movements from video data. This technology has a wide range of applications, including silent speech recognition, lip reading, and enhancing accessibility for individuals with hearing impairments. By leveraging state-of-the-art Tensorflow's Convolutional Neural Networks and OpenCV, Lip Net aims to provide accurate and real-time analysis of lip movements, transforming the way we interact with technology and improving communication for those with speech and hearing challenges.

## Motivation
The motivation behind Lip Net stems from the need to bridge communication gaps and provide innovative solutions for individuals who rely on visual cues for understanding speech. Traditional speech recognition systems rely heavily on audio input, which can be limiting in noisy environments or for individuals with hearing impairments. Lip Net addresses these limitations by focusing on visual data, offering a complementary approach to existing speech recognition technologies.

# Built With
* <img src= "https://img.shields.io/badge/TensorFlow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white"/>
* <img src="https://img.shields.io/badge/Keras-FF0000?style=for-the-badge&logo=keras&logoColor=white"/>
* <img src="https://img.shields.io/badge/Numpy-777BB4?style=for-the-badge&logo=numpy&logoColor=white"/>
* <img src="https://img.shields.io/badge/OpenCV-27338e?style=for-the-badge&logo=OpenCV&logoColor=white" />
* Matplotlib

# Installation 
```
git clone https://github.com/Char325/Lip-Net.git
cd Lip-Net
pip install -r requirements.txt

```
# Dataset 
* Database Installation can be done by running the following script:
```
import gdown
url=("https://drive.google.com/uc?id=1YlvpDLix3S-U8fd-gqRwPcWXAXm8JwjL")
output="data1.zip"
gdown.download(url,output,quiet=True)
gdown.extractall(output)
```
* Upon Installation, the zip file consists of two folders: alignments and s1. The alignment folder consists of the text per frames in a ```.align``` file. The s1 consists video files of about 1-2 seconds in ```.mpg``` format. There are about a total of 999 files in audio and text data respectively. An text file can be matched to the audio file using the name given. Consider the following video file ``` bbaf2n.mpg ```
 

https://github.com/user-attachments/assets/2f2f19a0-8b72-4561-9aeb-a5b921d7f7b8

 
  Its corresponding text is given by ``` bbaf2n.align```
  
  ![image](https://github.com/user-attachments/assets/a58fcf63-a22e-4f93-88d6-fac116308eac)


# How It Works
Lip Net consists of several key components that work together to achieve accurate lip movement analysis:

* #### Data Collection:
High-quality video data of individuals speaking is collected. This data serves as the foundation for training and testing the neural network models. This data is available as a Google Drive link within the code. 
* #### Preprocessing:
 The video data is preprocessed to extract relevant features, such as the region of interest (the lips) and key points that represent lip movements.
 A sample animation is:
 
 ![animation](https://github.com/user-attachments/assets/a2e58814-ee73-4ed3-af38-bc89c06e2f4a)

* #### Convolutional Neural Network Model:
A deep learning CNN model is trained on the preprocessed data. This model learns to recognize patterns in lip movements and associate them with corresponding phonemes or words.
* #### Inference:
During inference, the trained model analyzes new video data to interpret lip movements and generate text output or other relevant responses.

# Future Directions
Lip Net has several potential future directions:

* Improved Accuracy: Continuously refining the neural network models to improve the accuracy of lip movement recognition.
* Expanded Dataset: Collecting and incorporating more diverse datasets to ensure the system performs well across different languages, accents, and speaking styles.
* Integration with Other Technologies: Exploring the integration of Lip AI with other technologies, such as augmented reality (AR) and virtual reality (VR), to create more immersive and interactive experiences.
# Contributing
Guidelines for contributing to the project. For example:

1. Fork the repository
2. Create a new branch (git checkout -b feature-branch)
3. Make your changes
4. Commit your changes (git commit -m 'Add some feature')
5. Push to the branch (git push origin feature-branch)
6. Open a pull request

