# Motor-Imagery-Classification-from-time-domain-low-frequency-EEG-signals
The project's overarching objective is the development of a sophisticated deep neural network capable of accurately classifying EEG signals into motor impulses, thereby enabling the seamless execution of a range of actions integral to fundamental human rehabilitation after transhumeral amputation.
# Introduction
EEG-based robotic arm control has offered a key solution to the problem of high level amputation or severe neuromuscular damage. Several attempts to use EMG-based pattern recognition (PR) failed due to insufficient myoelectric signals from the residual limb to perform control functions. The EEG activity recorded from the human scalp is used to control the movement of a robotic arm. This can be achieved when the arm is either attached to or separated from the amputee stump by interfacing the brain directly to the robotic arm through the brain-machine interface (BMI). To build an intelligent robotic (or prosthetics) system that will manipulate object seamlessly with multiple degrees of freedom (DoF), it is required that a robust learning algorithm which is able to control the prosthetic arm while interacting with the environment should be implemented. However, the conventional machine learning approach of using handcrafted features to design a robot controller that can perform multiple tasks is not a feasible option. Hence, we propose a robust learning control which is based on a modified DeepConvNet with a classification accuracy of 56.25% on the BNCI Horizon 2020 dataset. The proposed approach has been selected after comparative analysis of EEGNet, DeepConvNet, HopefulNet and a self-made neural network in combination with different filtering techniques such as butterworth filter, firwin filter and common spatial filtering. Other methods such as using PyWavelet Transform were also compared. Our approach shows a better performance when compared with the state-of-the art classifiers. Thus, the proposed results demonstrate the possibility of providing better control performance for EEG-based prosthesis.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;


## :warning: Framework used

- [Python](https://www.python.org/)
- [MNE](https://mne.tools/stable/index.html)
- [EEGNet](https://eegnet.org/index.html)
- Epoch flex 32 EEG cap



