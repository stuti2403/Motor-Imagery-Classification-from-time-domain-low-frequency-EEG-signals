# Motor-Imagery-Classification-from-time-domain-low-frequency-EEG-signals
The project's overarching objective is the development of a sophisticated deep neural network capable of accurately classifying EEG signals into motor impulses, thereby enabling the seamless execution of a range of actions integral to fundamental human rehabilitation after transhumeral amputation.
# Introduction
EEG-based robotic arm control has offered a key solution to the problem of high level amputation or severe neuromuscular damage. Several attempts to use EMG-based pattern recognition (PR) failed due to insufficient myoelectric signals from the residual limb to perform control functions. The EEG activity recorded from the human scalp is used to control the movement of a robotic arm. This can be achieved when the arm is either attached to or separated from the amputee stump by interfacing the brain directly to the robotic arm through the brain-machine interface (BMI). To build an intelligent robotic (or prosthetics) system that will manipulate object seamlessly with multiple degrees of freedom (DoF), it is required that a robust learning algorithm which is able to control the prosthetic arm while interacting with the environment should be implemented. However, the conventional machine learning approach of using handcrafted features to design a robot controller that can perform multiple tasks is not a feasible option. Hence, we propose a robust learning control which is based on a modified DeepConvNet with a classification accuracy of 56.25% on the BNCI Horizon 2020 dataset. The proposed approach has been selected after comparative analysis of EEGNet, DeepConvNet, HopefulNet and a self-made neural network in combination with different filtering techniques such as butterworth filter, firwin filter and common spatial filtering. Other methods such as using PyWavelet Transform were also compared. Our approach shows a better performance when compared with the state-of-the art classifiers. Thus, the proposed results demonstrate the possibility of providing better control performance for EEG-based prosthesis.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;


## Overview

This repository hosts the code and resources for a research project focusing on the development of a novel approach for classifying Electroencephalogram (EEG) signals to enable enhanced control in neuroprostheses for individuals with transhumeral amputation. The project employs deep learning techniques and machine learning models to analyze EEG data collected during motor imagery tasks, facilitating the control of an exoskeletal arm for various movements.

## Table of Contents

- [Methodology](#methodology)
- [Data Set Description](#data-set-description)
- [Data Pre-processing](#data-pre-processing)
- [Model Creation](#model-creation)
- [Model Training](#model-training)
- [Model Testing](#model-testing)
- [Results](#results)

## Methodology

The methodology encompasses three primary phases:
1. **Data Collection and Preparation:** EEG data from 15 healthy subjects performing various upper limb movements and rest trials were collected and curated for analysis.
2. **Data Pre-processing:** Techniques including bandpass filtering, wavelet decomposition, and epoch extraction were employed to prepare the EEG data for model training.
3. **Model Development:** A modified DeepConvNet architecture was utilized to predict motor functions from EEG signals, after rigorous comparative analysis with other classification models like EEGNet and traditional DeepConvNet.
![diagram](https://github.com/stuti2403/Motor-Imagery-Classification-from-time-domain-low-frequency-EEG-signals/assets/72308729/6f82fdeb-e795-485a-8dad-568d4b07fa9c)


## Data Set Description

The dataset used comprises EEG recordings from 15 subjects performing six distinct upper limb movements, including elbow and wrist motions, and hand gestures. The data collection involved two sessions - physical movements and mental imagery, organized in GDF files with specific channel labeling.

## Data Pre-processing

The preprocessing pipeline involved extensive steps, such as bandpass filtering, event extraction, epoch creation, and data concatenation, to standardize and prepare the EEG data for model training.
![eeg preprocessing](https://github.com/stuti2403/Motor-Imagery-Classification-from-time-domain-low-frequency-EEG-signals/assets/72308729/c8aa0697-425b-4a14-8de8-20b91feadb4a)

## Model Creation

The modified DeepConvNet model, optimized through changes in batch normalization and kernel size, was designed to leverage the hierarchical features of EEG signals for accurate motor function prediction.
![arch_res_paper](https://github.com/stuti2403/Motor-Imagery-Classification-from-time-domain-low-frequency-EEG-signals/assets/72308729/b36ec08b-eea6-4edb-a5c4-d480e09c5873)

## Model Training

The model was trained using EEG signals from all subjects concatenated together. Various techniques and approaches, including different filtering methods and neural network architectures, were compared to achieve optimal training accuracy.

## Model Testing

Testing accuracy results demonstrated the superiority of the modified DeepConvNet model over EEGNet and traditional DeepConvNet, showcasing its capability to accurately classify motor functions from EEG data.

## Results

The project achieved significant advancements in EEG signal classification, outperforming existing techniques by approximately 27%. The proposed methodology shows promise in real-time EEG signal classification, offering potential applications in cutting-edge assistive technologies for individuals with transhumeral amputation.
Comparison of accuracy values obtained from DeepConvNet, EEGNet and modified DeepConvNet models:
![image](https://github.com/stuti2403/Motor-Imagery-Classification-from-time-domain-low-frequency-EEG-signals/assets/72308729/19205bed-36d5-40ee-b0d2-461c1908c917)



## Usage

To use the code and resources provided in this repository, follow the instructions in the respective directories. Detailed documentation and usage guidelines are included in each section of the project.

## Contributing

Contributions to this project are welcome! Please refer to the CONTRIBUTING.md file for guidelines on how to contribute.


## :warning: Framework used

- [Python](https://www.python.org/)
- [MNE](https://mne.tools/stable/index.html)
- [EEGNet](https://eegnet.org/index.html)



