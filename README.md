# Gesture-Based Slide Control System

## Project Overview

GestureSlide is a touch-free slide control system that allows users to control presentation slides using hand gestures.

The system uses a webcam to recognize the user’s hand gesture and converts the result into a keyboard command. A Shaka gesture moves the slide forward, while a fist gesture moves the slide backward.

## Motivation

In many real-world situations, directly touching a keyboard, mouse, or screen can be inconvenient or impossible.

For example, users may need hands-free control while cooking, exercising, conducting laboratory experiments, or giving a presentation.

This project aims to provide a simple and intuitive way to control slides without direct touch or additional hardware.

## Methods

The system follows this process:

Webcam → Image Processing → AI Prediction → Decision Logic → Keyboard Control

First, the webcam captures real-time video frames. Then, each image is resized and normalized so that it can be used as input for the AI model.

The trained model classifies the gesture into three classes: Next, Previous, or Background. After prediction, the system checks the confidence score, repeated frame recognition, and cooldown time to reduce accidental actions.

Finally, the recognized gesture is converted into a keyboard command to move the presentation slide forward or backward.

## Results

The system successfully recognized hand gestures and used them to control presentation slides.

The Shaka gesture was used to move to the next slide, and the fist gesture was used to move to the previous slide. Background gestures were used to prevent unintended slide actions.

The system also improved stability by using confidence scores, consecutive frame checks, and cooldown time.

## Team Members

* Siyeon Baek
* Gahyun Kim
