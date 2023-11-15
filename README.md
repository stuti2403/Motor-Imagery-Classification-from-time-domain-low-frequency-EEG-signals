# Motor-Imagery-Classification-from-time-domain-low-frequency-EEG-signals
The project's overarching objective is the development of a sophisticated deep neural network capable of accurately classifying EEG signals into motor impulses, thereby enabling the seamless execution of a range of actions integral to fundamental human rehabilitation after transhumeral amputation.
# Introduction
EEG-based robotic arm control has offered a key solution to the problem of high level amputation or severe neuromuscular damage. Several attempts to use EMG-based pattern recognition (PR) failed due to insufficient myoelectric signals from the residual limb to perform control functions. The EEG activity recorded from the human scalp is used to control the movement of a robotic arm. This can be achieved when the arm is either attached to or separated from the amputee stump by interfacing the brain directly to the robotic arm through the brain-machine interface (BMI). To build an intelligent robotic (or prosthetics) system that will manipulate object seamlessly with multiple degrees of freedom (DoF), it is required that a robust learning algorithm which is able to control the prosthetic arm while interacting with the environment should be implemented. However, the conventional machine learning approach of using handcrafted features to design a robot controller that can perform multiple tasks is not a feasible option. Hence, we propose a robust learning control which is based on a modified DeepConvNet with a classification accuracy of 56.25% on the BNCI Horizon 2020 dataset. The proposed approach has been selected after comparative analysis of EEGNet, DeepConvNet, HopefulNet and a self-made neural network in combination with different filtering techniques such as butterworth filter, firwin filter and common spatial filtering. Other methods such as using PyWavelet Transform were also compared. Our approach shows a better performance when compared with the state-of-the art classifiers. Thus, the proposed results demonstrate the possibility of providing better control performance for EEG-based prosthesis.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;

Certainly! A professional README file for a GitHub repository containing the project discussed in the research paper could look something like this:

---

# EEG-Based Neuroprosthesis Classification Project

## Overview

This repository hosts the code and resources for a research project focusing on the development of a novel approach for classifying Electroencephalogram (EEG) signals to enable enhanced control in neuroprostheses for individuals with transhumeral amputation. The project employs deep learning techniques and machine learning models to analyze EEG data collected during motor imagery tasks, facilitating the control of an exoskeletal arm for various movements.

## Table of Contents

- [Introduction](#introduction)
- [Methodology](#methodology)
- [Data Set Description](#data-set-description)
- [Data Pre-processing](#data-pre-processing)
- [Model Creation](#model-creation)
- [Model Training](#model-training)
- [Model Testing](#model-testing)
- [Results](#results)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Introduction

The research paper this project is based on addresses the need for improved control mechanisms in neuroprostheses for individuals experiencing limb amputation. The paper introduces a pioneering method that utilizes deep learning models for classifying EEG signals generated during motor imagery tasks, aiming to enhance the control of an exoskeletal arm.

## Methodology

The methodology encompasses three primary phases:
1. **Data Collection and Preparation:** EEG data from 15 healthy subjects performing various upper limb movements and rest trials were collected and curated for analysis.
2. **Data Pre-processing:** Techniques including bandpass filtering, wavelet decomposition, and epoch extraction were employed to prepare the EEG data for model training.
3. **Model Development:** A modified DeepConvNet architecture was utilized to predict motor functions from EEG signals, after rigorous comparative analysis with other classification models like EEGNet and traditional DeepConvNet.

## Data Set Description

The dataset used comprises EEG recordings from 15 subjects performing six distinct upper limb movements, including elbow and wrist motions, and hand gestures. The data collection involved two sessions - physical movements and mental imagery, organized in GDF files with specific channel labeling.

## Data Pre-processing

The preprocessing pipeline involved extensive steps, such as bandpass filtering, event extraction, epoch creation, and data concatenation, to standardize and prepare the EEG data for model training.

## Model Creation

The modified DeepConvNet model, optimized through changes in batch normalization and kernel size, was designed to leverage the hierarchical features of EEG signals for accurate motor function prediction.

## Model Training

The model was trained using EEG signals from all subjects concatenated together. Various techniques and approaches, including different filtering methods and neural network architectures, were compared to achieve optimal training accuracy.

## Model Testing

Testing accuracy results demonstrated the superiority of the modified DeepConvNet model over EEGNet and traditional DeepConvNet, showcasing its capability to accurately classify motor functions from EEG data.

## Results

The project achieved significant advancements in EEG signal classification, outperforming existing techniques by approximately 27%. The proposed methodology shows promise in real-time EEG signal classification, offering potential applications in cutting-edge assistive technologies for individuals with transhumeral amputation.

## Usage

To use the code and resources provided in this repository, follow the instructions in the respective directories. Detailed documentation and usage guidelines are included in each section of the project.

## Contributing

Contributions to this project are welcome! Please refer to the CONTRIBUTING.md file for guidelines on how to contribute.

## License

This project is licensed under the [INSERT LICENSE NAME] License - see the LICENSE.md file for details.

---

Ensure to replace placeholders such as "[INSERT LICENSE NAME]" with the appropriate license name used in your project. Additionally, link relevant sections to corresponding files or directories within your repository. This README provides a comprehensive overview of the project structure, methodologies, and outcomes, enabling users and contributors to understand and engage with the research work effectively.
## :warning: Framework used

- [Python](https://www.python.org/)
- [MNE](https://mne.tools/stable/index.html)
- [EEGNet](https://eegnet.org/index.html)



