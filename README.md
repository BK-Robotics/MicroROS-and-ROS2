# MicroROS-and-ROS2
Using MicroROS and ROS2 to setup communication between host computer and microcontroller (STM32F411E - Disco board)

## About this project
I am using STM32CubeIDE - FreeRTOS to setup MicroROS library to STM32F411

This project is just upload MicroROS library to the STM32F411 microcontroller and make a communication to laptop through USB serial

However, please remember that I haven't write any MicroROS application yet! And the built-in blue LED should blink after 1s.

Ubuntu 22.04LTS

STM32CubeIDE

## Prerequisites:
I will update this based on the bugs that people get :)
1. CH340 Driver

## If you want to flash to STM32, follow these steps:
1. Clone the repo to your own local folder
2. Open STM32CubeIDE and find the workspace in repo folder
3. Build the F411 Disco2 project
4. Debug the F411 Disco2 project then run it

### Check the connection:
`ls /dev/tty*`

Look for `/dev/ttyCH341USB0` (This only show if you had successfully install CH340 driver, otherwise, it will be ttyUSB0)

`sudo screen /dev/ttyCH341USB0 115200`

This line should show the string "Hello, computer!" after entered.
