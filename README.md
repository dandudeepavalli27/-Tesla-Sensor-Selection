# TESLA (Sensor Selection)

## Aim
To analyze sensor range metadata using the KITTI Vision Benchmark Dataset and select the most suitable sensor for autonomous vehicle perception based on maximum sensing range.

---

## Dataset
KITTI Vision Benchmark Dataset  
Link: http://www.cvlibs.net/datasets/kitti/

Calibration and sensor-related metadata from the KITTI dataset are used as reference for sensor selection.

---

## Objective
Autonomous vehicles use multiple sensors such as Camera, Radar, LiDAR, and Ultrasonic sensors. Each sensor has different sensing ranges and capabilities. The objective of this experiment is to compare the sensing ranges and select the sensor with the maximum range for better environment perception.

---

## Procedure
Step 1: Download the KITTI dataset calibration or sensor metadata files.

Step 2: Upload the dataset into the coding environment (Google Colab / Python / Jupyter Notebook).

Step 3: Define the available sensors and their sensing ranges.

Step 4: Read and store the sensor range values.

Step 5: Compare the sensing range of all sensors.

Step 6: Identify the sensor with the maximum sensing range.

Step 7: Display the selected sensor.

---

## Algorithm

Step 1: Start the program.

Step 2: Load the KITTI dataset or define the sensor metadata.

Step 3: Define the sensors used in autonomous vehicles:
        Camera
        Radar
        LiDAR
        Ultrasonic Sensor

Step 4: Assign sensing range values (in meters) to each sensor.

Step 5: Store sensor names and range values in a dictionary or list.

Step 6: Initialize a variable to store the maximum range.

Step 7: Compare each sensor range with the current maximum range.

Step 8: If the current sensor range is greater than the maximum range:
        Update the maximum range value.
        Store the sensor name.

Step 9: Repeat until all sensors are compared.

Step 10: Select the sensor with the highest sensing range.

Step 11: Display the selected sensor.

Step 12: Output the result.

Step 13: Stop the program.

---

## Code Logic

if sensor_range == maximum_range:
    selected_sensor = "LiDAR"

---

## Python Implementation

```python
# Sensor range values in meters

sensors = {
    "Camera": 80,
    "Radar": 150,
    "LiDAR": 200,
    "Ultrasonic": 10
}

# Select sensor with maximum range
selected_sensor = max(sensors, key=sensors.get)

print("Selected Sensor:", selected_sensor)# -Tesla-Sensor-Selection
