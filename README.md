<p align="center">
<img src="Resource/awesome-ml-demos-with-ios-logo.png" width="187" height="174"/>
</p>


[![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/motlabs/awesome-ml-demos-with-ios) [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](http://makeapullrequest.com) [![GIF PRs More Welcome](https://img.shields.io/badge/GIF--PRs-WELCOME!-brightgreen.svg?style=flat-square)](http://makeapullrequest.com)

# Awesome Machine Learning DEMOs with iOS

We tackle the challenge of using machine learning models on iOS via Core ML and ML Kit (TensorFlow Lite).

[한국어 README](https://github.com/motlabs/iOS-Proejcts-with-ML-Models/blob/master/README_kr.md)

## Contents
- [Machine Learning Framework for iOS](#machine-learning-framework-for-ios)
  - [Flow of Model When Using Core ML](#Flow-of-Model-When-Using-Core-ML)
  - [Flow of Model When Using Create ML](#Flow-of-Model-When-Using-Create-ML)
- [Baseline Projects](#Baseline-Projects)
  - [Image Classification](#Image-Classification)
  - [Pose Estimation](#Pose-Estimation)
  - [Object Detection & Recognition](#Object-Detection--Recognition)
- [Application Projects](#Application-Projects)
  - [Annotation Tool](#Annotation-Tool)
- [Create ML Projects](#Create-ML-Projects)
- [Performance](#Performance)
  - [📏Measure module](#measure-module)
  - [Implements](#Implements)
- [See also](#See-also)

## Machine Learning Framework for iOS

- [Core ML](https://developer.apple.com/documentation/coreml)
- [ML Kit](https://developers.google.com/ml-kit/)
- [fritz](https://www.fritz.ai/)
- etc. ([Tensorflow Lite](https://www.tensorflow.org/mobile/tflite/), ~~[Tensorflow Mobile](https://www.tensorflow.org/mobile/)~~`DEPRECATED`)


### Flow of Model When Using Core ML

[![Flow of Model When Using Core ML](Resource/flow_of_model_when_using_coreml.png?raw=true)](https://docs.google.com/presentation/d/1wA_PAjllpLLcFPuZcERYbQlPe1Ipb-bzIZinZg3zXkg/edit?usp=sharing)

The overall flow is very similar for most ML frameworks. Each framework has its own compatible model format. We need to take the model created in TensorFlow and **convert it into the appropriate format, for each mobile ML framework**.

Once the compatible model is prepared, you can run the inference using the ML framework. Note that you must perform **pre/postprocessing** manually.

> If you want more explanation, check [this slide(Korean)](https://docs.google.com/presentation/d/1wA_PAjllpLLcFPuZcERYbQlPe1Ipb-bzIZinZg3zXkg/edit?usp=sharing).

### Flow of Model When Using Create ML

![playground-createml-validation-001](Resource/flow_of_model_when_using_createml.png)

## Baseline Projects

#### DONE

- Using built-in model with Core ML

- Using built-in on-device model with ML Kit
- Using custom model for Vision with Core ML and ML Kit
- Object Detection with Core ML

#### TODO

- Object Detection with ML Kit
- Using built-in cloud model on ML Kit
  - Landmark recognition
- Using custom model for NLP with Core ML and ML Kit
- Using custom model for Audio with Core ML and ML Kit
  - Audio recognition
  - Speech recognition
  - TTS



### Image Classification

| Name | DEMO | Note |
| ---- | ---- | ---- |
| [ImageClassification-CoreML](https://github.com/tucan9389/ImageClassification-CoreML) | <p align="center"><img src="Resource/MobileNet-CoreML-DEMO.gif" width="200"/></p> | - |
| [MobileNet-MLKit](https://github.com/tucan9389/MobileNet-MLKit) | <p align="center"><img src="Resource/MobileNet-MLKit-DEMO.gif" width="200"/></p> | - |

### Pose Estimation

| Name | DEMO | Note |
| ---- | ---- | ---- |
| [PoseEstimation-CoreML](https://github.com/tucan9389/PoseEstimation-CoreML) | <p align="center"><img src="Resource/180801-poseestimation-demo.gif" width="200"/></p> | - |
| [PoseEstimation-MLKit](https://github.com/tucan9389/PoseEstimation-MLKit) | <p align="center"><img src="Resource/PoseEstimation-MLKit-hourglass.gif" width="200"/></p> | - |
| [FingertipEstimation-CoreML](https://github.com/tucan9389/FingertipEstimation-CoreML) | <p align="center"><img src="Resource/fingertip_estimation_demo003.gif" width="200"/></p> | - |

### Object Detection & Recognition

| Name | DEMO | Note |
| ---- | ---- | ---- |
| [SSDMobileNet-CoreML](https://github.com/tucan9389/SSDMobileNet-CoreML) | <p align="center"><img src="Resource/SSDMobileNetV2-DEMO.gif" width="200"/></p> | - |
| [TextDetection-CoreML](https://github.com/tucan9389/TextDetection-CoreML) | <p align="center"><img src="Resource/TextDetection-CoreML_DEMO001.gif" width="200"/></p> | - |
| [TextRecognition-MLKit](https://github.com/tucan9389/TextRecognition-MLKit) | <p align="center"><img src="Resource/TextRecognition-MLKit_DEMO002.gif" width="200"/></p> | - |
| [FaceDetection-MLKit](https://github.com/tucan9389/FaceDetection-MLKit) | <p align="center"><img src="Resource/FaceDetection-MLKit-DEMO.gif" width="200"/></p> | - |

## Application Projects

| Name | DEMO | Note |
| ---- | ---- | ---- |
| [dont-be-turtle-ios](https://github.com/motlabs/dont-be-turtle-ios) | <p align="center"><img src="Resource/dont-be-turtle_demo_004.gif" width="200"/></p> | - |
| [WordRecognition-CoreML-MLKit](https://github.com/tucan9389/WordRecognition-CoreML-MLKit)(preparing...) | <p align="center"><img src="Resource/recognition_a_word_demo002.gif" width="200"/></p> | Detect character, find a word what I point and then recognize the word using Core ML and ML Kit. |

### Annotation Tool

| Name | DEMO | Note |
| ---- | ---- | ---- |
| [KeypointAnnotation](https://github.com/tucan9389/KeypointAnnotation) | <p align="center"><img src="Resource/annotation_ios_app_demo001.gif" width="200"/></p> | Annotation tool for own custom estimation dataset |

## Create ML Projects

| Name | Create ML DEMO | Core ML DEMO | Note |
| ------ | ------------------------------------------------------------ | ---------------------------------- | ------ |
| [SimpleClassification-CreateML-CoreML](https://github.com/tucan9389/SimpleClassification-CreateML-CoreML) | ![IMG_0436](Resource/playground-createml-validation-001.png) | ![IMG_0436](Resource/IMG_0436.PNG) | A Simple Classification Using Create ML and Core ML |

## Performance

Execution Time: Inference Time + Postprocessing Time

|              (with iPhone X) | Inference Time(ms) | Execution Time(ms) |   FPS   |
| ---------------------------: | :----------------: | :----------------: | :-----: |
|   ImageClassification-CoreML |         40         |         40         |   23    |
|              MobileNet-MLKit |        120         |        130         |    6    |
|        PoseEstimation-CoreML |         51         |         65         |   14    |
|         PoseEstimation-MLKit |        200         |        217         |    3    |
|          SSDMobileNet-CoreML |  100 ~ 120         |    110 ~ 130       |    5    |
|         TextDetection-CoreML |         12         |         13         | 30(max) |
|        TextRecognition-MLKit |       35~200       |       40~200       |  5~20   |
| WordRecognition-CoreML-MLKit |         23         |         30         |   14    |
| FaceDetection-MLKit          |         -          |          -         |   -     |

### 📏Measure module

You can see the measured latency time for inference or execution and FPS on the top of the screen.

> If you have more elegant method for measuring the performance, suggest on issue!

<img src="Resource/measure_ui.jpeg" width="320"/>

### Implements

|                       | Measure📏 | Unit Test | Bunch Test |
| --------------------: | :-------: | :-------: | :--------: |
| ImageClassification-CoreML | O    |     X     |     X      |
|       MobileNet-MLKit |    O      |     X     |     X      |
| PoseEstimation-CoreML |    O      |     O     |     X      |
|  PoseEstimation-MLKit |    O      |     X     |     X      |
|   SSDMobileNet-CoreML |    O      |     O     |     X      |
|  TextDetection-CoreML |    O      |     X     |     X      |
| TextRecognition-MLKit |    O      |     X     |     X      |

## See also

- [Core ML | Apple Developer Documentation](https://developer.apple.com/documentation/coreml)
- [Machine Learning - Apple Developer](https://developer.apple.com/machine-learning/)
- WWDC17 - Core ML
  - [WWDC17 703 Session - Introducing Core ML](https://developer.apple.com/videos/play/wwdc2017/703/)
  - [WWDC17 710 Session - Core ML in depth](https://developer.apple.com/videos/play/wwdc2017/710/)
  - [WWDC17 506 Session - Vision Framework: Building on Core ML](https://developer.apple.com/videos/play/wwdc2017/506)
- WWDC18 - Core ML 2
  - [WWDC18 708 Session - What’s New in Core ML, Part 1](https://developer.apple.com/videos/play/wwdc2018/708/)
  - [WWDC18 709 Session - What’s New in Core ML, Part 2](https://developer.apple.com/videos/play/wwdc2018/709/)
  - [WWDC18 717 Session - Vision with Core ML](https://developer.apple.com/videos/play/wwdc2018/717/)
- [ML Kit - Firebase](https://developers.google.com/ml-kit/)
- [Apple's Core ML 2 vs. Google's ML Kit: What's the difference?](https://venturebeat.com/2018/06/05/apples-core-ml-2-vs-googles-ml-kit-whats-the-difference/)
- [iOS에서 머신러닝 슬라이드 자료](https://docs.google.com/presentation/d/1wA_PAjllpLLcFPuZcERYbQlPe1Ipb-bzIZinZg3zXkg/edit?usp=sharing)
- [MoTLabs Blog](https://motlabs.github.io/)
