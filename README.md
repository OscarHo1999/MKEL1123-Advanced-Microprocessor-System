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





   
