**Earthquake Detector**

**Overview**

This project is a simple earthquake detection system built using Arduino and C++. It uses a 3-axis ADXL335 accelerometer to detect vibration, shaking, or tilt that could represent seismic activity. If the system detects strong movement, it triggers an alert using a buzzer and LED.

An LCD screen shows the real time sensor values so the user can see motion changes along the X, Y, and Z axes.

I built this project on my own to learn how motion sensors and embedded systems can be used to detect real world events.

**Hardware Used**

- Arduino board
- ADXL335 3-axis accelerometer
- 16x2 LCD display with I2C module
- LED
- Buzzer
- 330 ohm resistor
- Jumper wires

**Software**

**Programming language**

Arduino C++

**Development tool**

Arduino IDE

**For data visualization**

- Python

- matplotlib

**How the System Works**

The ADXL335 sensor measures acceleration across three axes.

When the system starts, it first performs a calibration step. The Arduino collects several samples and calculates baseline values for the X, Y, and Z axes.

After calibration, the system continuously reads the sensor values.

If the change in acceleration exceeds a selected threshold, the system assumes strong vibration has occurred.

When that happens:

- the LED turns on
- the buzzer sounds an alert
- the LCD displays an earthquake warning

The sensor values are also sent to the serial monitor.

These readings can be exported and plotted using Python and matplotlib to visualize vibration intensity.

**Features**

- vibration detection using a 3-axis accelerometer
- automatic calibration for stable baseline readings
- real time display of X, Y, and Z motion values
- LED and buzzer alert system
- vibration data visualization using Python

**What I Learned**

From this project I learned:

- how accelerometers detect motion and tilt
- how to process multi axis sensor data
- how calibration improves sensor accuracy
- how microcontrollers interact with sensors and displays
- how hardware sensor data can be visualized using Python

**Future Improvements**

Possible improvements include:

- storing vibration data for long term monitoring
- wireless alerts using IoT modules
- improving sensitivity for smaller vibrations

