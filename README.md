﻿# Sign Language to english
#### Code owner is Youtuber Nicholas Renotte (https://github.com/nicknochnack). Modified Action Detection code to capture American Sign Language and translate it to English

The ASL to English Translation Model you developed is a practical computer vision system for translating American Sign Language gestures into English text, potentially transforming accessibility for those who use ASL as a primary mode of communication.

### Project Overview

1. **Objective**: The project aimed to create a real-time system that detects and translates ASL gestures to English, facilitating communication between ASL users and non-signers. This proof of concept focused on three specific ASL gestures, demonstrating the feasibility of real-time sign language interpretation.

2. **Technical Workflow**:
   - **Skeletal Tracking with MediaPipe**: The model captures skeletal keypoints (1,662 features) in each frame, tracking hand and body movements crucial for interpreting ASL.
   - **Gesture Recognition via LSTM**: A custom LSTM neural network (596,675 parameters) processes sequences of skeletal features, which is essential for recognizing temporal patterns in ASL gestures. LSTM is ideal here as it excels in handling sequential data, allowing for accurate gesture detection over time.
   - **Real-Time Inference and Visualization**: Using OpenCV, the model processes video frames in real time, displaying translation results along with a probability indicator to convey the confidence level of each prediction.

3. **Dataset**: A custom dataset of 2,700 frames was collected, structured into 30 sequences of 30 frames for each of the 3 gestures. This dataset structure allows the model to learn gesture transitions and dynamics accurately.

### Potential Applications

1. **Assistive Technology for Accessibility**:
   - Real-time ASL translation can assist individuals who are deaf or hard of hearing by bridging communication gaps with non-signers. For instance, the model can be integrated into mobile applications or embedded devices to support everyday communication in public spaces, workplaces, and service areas.
  
2. **Education and Learning**:
   - This system could serve as an educational tool for people learning ASL, providing instant feedback on gesture accuracy and aiding in vocabulary building by translating signed gestures into English words.

3. **Interactive Interfaces**:
   - The model could be extended to support a broader range of gestures and applied in gesture-based user interfaces, where users control software applications or devices through ASL gestures, providing a touch-free, accessible interaction method.

4. **Research and Development in ASL Recognition**:
   - With the foundational ML pipeline you've built, researchers can extend the dataset, expand gesture vocabulary, and refine the model for more complex ASL recognition tasks, moving closer to achieving continuous ASL-to-text translation.

This project demonstrates how real-time gesture recognition combined with deep learning can make significant strides in enhancing communication and accessibility through innovative computer vision solutions.

