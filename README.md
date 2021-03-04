# Tello-Python

## Introduction

This is a collection of python-based sample code that interacts with the Ryze Tello drone.

## Project Description

This toolkit contains three sample programs based on the Tello SDK, using Python (version 2.7). This comprises of `Single_Tello_Test`, `Tello_Video`, and `Tello_Video(With_Pose_Recognition)`. There is also another program `tello_state.py`, which receives and prints the current state of the Tello.

- **Single_Tello_Test**

In `Single_Tello_Test`, you can design a series of command combinations by writing a text script, which the Tello will then execute. This program can also be used to test commands for the Tello.

- **Tello_Video**

In `Tello_Video`，you can receive the video stream data from tello, decode the video through the H264 decoding library, and display it on a GUI interface based on `Tkinter` and `PIL` (Python Imaging Library). In addition, it also supports a control panel which can operate the Tello. The sample code provided shows an example of receiving, processing and fetching the correct video data. The source code for the H264 decoding library is also provided in the package, which can be used for reference.

- **Tello_Video(With_Pose_Recognition)**

`Tello_Video_With_Pose_Recognition` is an application modified from Tello_Video. It uses the decoded video data and extracts frames for pose recognition. It also binds specific posture and aircraft SDK commands which allows pose control of Tello. This code is mainly used as an sample case for utilizing the decoded video stream of the Tello for image processing.

- **Tello_state.py**

`Tello_state.py` reads the various status data of the tello

## Environmental configuration

The sample code mentioned above is based on Python 2.7. There is no need to install additional third-party libraries for running `Single_Tello_Test` and `tello_state.py`. For `Tello_Video` and `Tello_Video(With_Pose_Recognition`), you need to install a series of third-party libraries. Therefore, in these two folders, one-click installation scripts (for Windows 32/64, Linux and macOS) are provided, which can assist you with installing all the relevant dependencies.

For more information specific to the content and description of each package, you can refer to the `README` file in the related folder. 

## Contact Information

If you have any questions about this sample code and the installation, please feel free to contact me. You can communicate with me by sending an e-mail to sdk@ryzerobotics.com.

Please note that we have recently committed a new FAQ file to the root of this repository. If you have any questions, please check that file first.

## About Multi-Tello-Formation

For controlling multiple drones at once, please refer to the GitHub repository at https://github.com/TelloSDK/Multi-Tello-Formation, which contains information and code specific to multi-tello swarms. 
