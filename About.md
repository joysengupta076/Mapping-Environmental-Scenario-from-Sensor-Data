# Abstract

This project showcases how to generate the surrounding environmental / virtual driving scenario from recorded sensor data on a participating ego vehicle or mobile robot.
In this case, the real scenario was generated with the help of data from GPS sensor and Lidar object lists. The setup consists of an onward facing camera, GPS Sensors and Lidar sensors mounted on an ego vehicle. ASAM OpenDRIVE files are used to convert geographical map data to virtual path data that can be modeled as per our needs
digitally. The digital path structures or road network are created in this form and visualize the real world virtually. It can be somewhat called 'Reverse-Engineering'.

## Methodology
The following steps were performed in this project:

- Recorded Sensor data from the sensors onboard the ego-vehicle / mobile robot were collected.

- ASAM OpenDRIVE road network was imported into driving scenario as an object.

- Firstly the ego-vehicle was modeled using the GPS data and recreated in the driving scenario.

- Second, the non-ego actors (here bus, bike, truck etc.) from lidar object list were modeled and recreated in the driving scenario.

- The speed, trajectory, heading angles etc. were modeled using waypoints, coordinates, sensor timestamps and the same was done.

- For validation, the reference video output data from the onboard camera can be used to verify the closeness of the generated scenario to the realworld situation.


## Motivation

Virtual environment recreations or path scenarios can be used to recreate a real scenario from recorded sensor data on a mobile robot or vehicle. Such virtual scenarios 
can help us to visualize and study the original scenario. We can also use them to synthesize scenario variations when designing and evaluating autonomous driving 
systems especially for recreating accident or testing scenarios because we can programmatically modify virtual situations by parameters and other changes. 
