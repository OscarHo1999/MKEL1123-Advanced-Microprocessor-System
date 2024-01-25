# MKEL1123-Advanced-Microprocessor-System
# Image Processing on STM32 Using CMSIS-NN

* [Introduction](#Introduction "Goto Introduction")
    * [MNIST Dataset](#MNIST-Dataset)
    * [Hardware](#Hardware "Goto Hardware")
    * [Software](#Software)
* [Pinout & Configuration](#pinout-and-configuration)
 
     


## Introduction

<div style="text-align: justify"> This initiative explores the implementation of image recognition using TensorFlow Lite for Microcontrollers (TFLM) and CMSIS-NN on the Discovery STM32Nucleo-F446RE board. The project is designed to facilitate accuracy and performance testing on any embed-enabled device accommodating the final binary. The model, trained on the MNIST dataset, a database of handwritten digits has a training set of 60,000 examples, and a test set of 10,000 examples. The methodology involves implementing CMSIS-NN on the STM32F44RE Nucleo board, leveraging its CORTEX-M4 core with SIMD and DSP capabilities. The project processes computer-sourced images on the microcontroller, utilizing the ARM Cortex M4's ART accelerator and FPU over Flash memory. Key steps include neural network configuration, code generation, library integration, and inference execution. The output is transmitted to the computer for tabulation. CMSIS-NN optimization aims to enhance efficiency in neural network inference and image processing tasks, optimizing pixel format conversion for memory efficiency. The Cortex-M4's limitations in memory and cache size contrast with its energy efficiency. 

### MNIST Dataset
![image](https://github.com/OscarHo1999/MKEL1123-Advanced-Microprocessor-System/assets/67437888/80c1c562-9761-43b4-b067-d2a1daa8906f)

In this project, the dataset that we used is MNIST dataset. MNIST, which is Modified National Institute of Standards and Technology database, consisting a collection of 70,000 28x28 pixels images of handwritten digits from 0 to 9. There are 60,000 training examples and 10,000 testing examples.

### Hardware
* [STM32F446RE](https://my.element14.com/stmicroelectronics/nucleo-f446re/dev-board-arduino-mbed-nucleo/dp/2491978)

### Software
* [STM32 Cube IDE](https://www.st.com/en/development-tools/stm32cubeide.html)
* [CMSIS NN Library](https://www.keil.com/pack/doc/cmsis/NN/html/index.html)

## Pinout and Configuration

Laptop output | Board Pinout
------------ | -------------
USB | USART


![image](https://github.com/OscarHo1999/MKEL1123-Advanced-Microprocessor-System/assets/67437888/461fa807-8fdc-47c4-8ad6-d18efc94c5d3)
To train and validate the model onto the board, we are use STM32CubeIDE in conjunction with the STM32 X-Cube-AI tools. The STM32 X-CUBE-AI bundle within the IDE's libraries and plugins. Models trained with TensorFlow, Keras, etc. are supported. With the tools, we can code the microcontroller to do inference—that is, our image recognition for digit numbers—after loading the learned model into it. After setting up the model, we can apply the MNIST model to CubeAI and produce code using the model framework. The MNIST database has also been generated for the project.

![image](https://github.com/OscarHo1999/MKEL1123-Advanced-Microprocessor-System/assets/67437888/427b4c01-f46f-490a-81b7-a85d45c297b6)
The trained model in our study uses the MNIST dataset to construct a digit recognition system. We must train the model into our board by utilizing the pre-trained model. To make sure the board has adequate flash to support the model, we must examine the model before we can begin training it.

![image](https://github.com/OscarHo1999/MKEL1123-Advanced-Microprocessor-System/assets/67437888/c42811b5-39d3-47dd-b8c2-cd4d086ee440)
We have validated the model to make sure it can be used in the board by connecting the board to the laptop.







   
