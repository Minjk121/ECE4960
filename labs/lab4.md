---
layout: default
---

# Lab 4: Characterize your car

The goal of the lab is to understand the characteristics and capabilities of the robot before adding motor drive driver for the future labs. 
Before this lab, the Artemis board, IMU and TOF sensors were soldered and connected.

Force 1 Cyclone Remote Control Car was used with 600mAh and 850mAh battery packs. 

### Category A: Simple Measurements

Simple measurements were collected without any control of the car. Its length, width and wheel diameter are measured as shown in the manual below.

![manual](https://github.com/Minjk121/ECE4960/blob/c7822b680428b86b536d338eee6e507c0075e754/img/manual_pic.jpg)

For the tools, tape measurement, ruler and food scale were used.

![car with ruler](img4/length.jpg)
![car on scale](img4/weight.jpg)

|  Length (cm)  |   Width (cm)  |  Height (cm)  |   Weight (g)  | Wheel Diameter (cm) | 
| ------------- | ------------- | ------------- | ------------- | ------------------- | 
|     17.9      |     14.2      |      7.9      |      499      |         7.9         | 

After collecting the static measurements, we measured average rotational speed with 850mAh by pressing right botton on the remote control and analyzing the timestamps in the video. We then used a fully charged 850mAh battery to controlled the car to rotate and measured the battery life time until it stops with stopwatch. The car shaked and could not be controlled once the battery is out. 

![850mah battery](img4/850mAh.jpg)

We tried to measure the charging time; however, it took too long to charge. We calculated the estimate charging time by measuring the current with a multimeter which measured to be 50mA. To fully charge the 850mAh battery, it will estimately take 17 hours. 

![tools](img4/tools.jpg)

|   Average Rotational speed  |  Battery Time (s) | Est. Charging Time (s) |
| --------------------------- | ----------------- | ---------------------- |
|         4.0 rev/sec         |  7 min 52.9 sec   |         17 hrs         |



### Category B: Experimental Setups

Using 600mAh, braking distance and decceletaion were measured on the tile in Phillips Hall.
*video*

|   Tests on Tile    | Braking Distance (ft) | Braking Time (s) | Deceleration (ft/m^2) |
| ------------------ | --------------------- | ---------------- |---------------------- |
| Average Measurement|          4.667        |      1.21        |          6.375        |

The tests were conducted with different conditions such as 850 mAh battery and carpet; however, the braking distance could not be measured because the car was flipped instead of braking due to the change in battery and higher resistance on the surface. 

The 850mAh battery was used for the rest of the tests. 

*video*

|         Tests       | Max Speed on Tile(ft/s) | Max Speed on Carpet (ft/s) | 
| ------------------- | ----------------------- | -------------------------- |
| Average Measurement |           11.96         |             11.76          |




Stunts: Flipping & Rotation & auto trick & drift

*videos*
