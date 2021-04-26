# Age Gender Raspberry Pi 4
![output image]( https://qengineering.eu/images/AgeGender4.jpg )
## Age and gender estimation with the OpenCV framework. <br/>
[![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)<br/><br/>
Paper: https://talhassner.github.io/home/publication/2015_CVPR<br/><br/>
Special made for a bare Raspberry Pi 4, see [Q-engineering deep learning examples](https://qengineering.eu/deep-learning-examples-on-raspberry-32-64-os.html)

------------

## Benchmark.
RPi 4 64-OS 1950 MHz <br/>
FPS = 1/(0.2 * Faces + 0.157)

------------

## Dependencies.
To run the application, you have to:
- A raspberry Pi 4 64-bit operating system. It can be the Raspberry 64-bit OS, or Ubuntu 18.04 / 20.04. [Install 64-bit OS](https://qengineering.eu/install-raspberry-64-os.html) <br/>
- OpenCV 64 bit installed. [Install OpenCV 4.5](https://qengineering.eu/install-opencv-4.5-on-raspberry-64-os.html) <br/>
- Code::Blocks installed. (```$ sudo apt-get install codeblocks```)

------------

## Installing the app.
To extract and run the network in Code::Blocks <br/>
$ mkdir *MyDir* <br/>
$ cd *MyDir* <br/>
$ wget https://github.com/Qengineering/Age-Gender-OpenCV-Raspberry-Pi-4/archive/refs/heads/main.zip <br/>
$ unzip -j master.zip <br/>
Remove master.zip, LICENSE and README.md as they are no longer needed. <br/> 
$ rm master.zip <br/>
$ rm LICENSE <br/>
$ rm README.md <br/> <br/>
Your *MyDir* folder must now look like this: <br/> 
sample1.jpg <br/>
sample3.jpg <br/>
AgeGender.cpb <br/>
AgeGender.cpp <br/>
opencv_face_detector.pbtxt <br/>
opencv_face_detector_uint8.pb <br/>
gender_deploy.prototxt <br/>
age_deploy.prototxt <br/><br/>
Do **not forget** to download the caffe models!

------------

## Running the app.
Download [age_deploy.caffemodel](https://drive.google.com/file/d/1pNDFo7WBcf4fo5DefGEbM01TJP8_z5H5/view?usp=sharing) <br/>
Download [gender_deploy.caffemodel](https://drive.google.com/file/d/1X8_2hTEUGculDA9gt_pIyTV31CNew8_b/view?usp=sharing) <br/>
To run the application load the project file YoloV5.cbp in Code::Blocks.<br/> 
Next, follow the instructions at [Hands-On](https://qengineering.eu/deep-learning-examples-on-raspberry-32-64-os.html#HandsOn).<br/><br/>
Many thanks to [GilLevi](https://github.com/GilLevi/AgeGenderDeepLearning) <br/>
TensorFlow implementation [dpressel](https://github.com/dpressel/rude-carnie)

