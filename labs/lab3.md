---
layout: default
---


# Lab 3: Sensors
![sensor](img3/soldered_parts.jpg)

The goal of the lab is to test sensors and equip the robot. In this lab, we will discuss and focus on the Time-of-Flight Sensors (ToF or VL53L1X) and the Inertial Measurement Unit (IMU). We will measure distance with ToF sensors and rotations (pitch/roll/yaw) with IMu sensor. The datasheetcan be found [here](https://cdn.sparkfun.com/assets/8/9/9/a/6/VL53L0X_DS.pdf) for ToF and [here](https://www.digikey.com/en/products/detail/pimoroni-ltd/PIM448/10246391) for IMU.

## Prelab: Wiring Connections

Before starting the lab, it is important to think about how to connect all the parts: Artemis Nano, two ToF sensors, and IMU sensor. Based on the datasheet, we know that sensor has I2C interface. This means the address will be the same for both sensors connected to the board. There are two ways to solve this problem and call each sensor: (1) changing the address by programming or (2) using shutdown pins (XSHUT). 

I chose to use the shutdown pins and draw the wiring schematics before the lab as shown below: 
![wiring](img3/wiring.jpg)

As we use [Qwiic cable](https://www.sparkfun.com/products/14426), we can connect Power, Ground, SDA, and SCL pins in the ToF sensors to the Artemis board closely. It is important to make sure all the pins are connected to the same pins in other boards. I connected shutdonw pins from the sensors to A0 and A1 pin in the board, considering the location of each part in the car. Based on the drawing, I soldered all the parts and wires together. 

## Time of Flight (ToF) Sensors

![tof](img3/TOF.jpg)

1. By running Eample05_Wire_I2C file, the I2C addresss of ToF was outputted as 0x29, as expected. 

2. The ToF sensor has three modes: ``` .setDistanceModeShort(), .setDistanceModeMedium(), .setDistanceModeLong(); ```
According to the [datasheet](https://cdn.sparkfun.com/assets/8/9/9/a/6/VL53L0X_DS.pdf), the short distance mode is more immune to ambient light but limied to 1.3m, and the long mode have a limit of 4m but impacted by ambient light. The medium mode is middle-ranging and gets an average impact of ambient light, comparing to the short and long modes.



## Inertial Measurement Unit (IMU)

1. 

