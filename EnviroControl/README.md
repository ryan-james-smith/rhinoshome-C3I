# EnviroControl

EnviroControl is a versatile project designed to enhance Home Assistant integration with a variety of environmental sensors and controls. It is based on a Leonardo R3 microcontroller and aims to provide smart, efficient monitoring and control of water levels, garden bed conditions, and other environmental factors.

**NOTE:** As with everything in this repository it has been specifically designed and put together for my use case with what i have lying around, if you just try to plug and play without taking the time to understand code and modify it to match your hardware configuration you will kill things from from your hardware to your stuff to you.
This is for competent people to take inspiration from not for people to use as is.

## Features

- **Water Level Monitoring**: Uses DFRobot SEN0257 Gravity Water Pressure Sensors to monitor the water levels in tanks.
- **Pump Control**: Controls the liquid level sensor/pump, acting as the float switch on a Matelec FPC_12650.
- **Garden Bed Monitoring**: Additional inputs can be used for soil moisture, pH, temperature, and other relevant sensors.
- **Home Assistant Integration**: Seamless integration with Home Assistant for real-time monitoring and control.

## Hardware Components

- **Microcontroller**: Leonardo R3
- **Network Shield**: DFRobot W5500 PoE Shield
- **Water Pressure Sensors**: DFRobot SEN0257 Gravity Water Pressure Sensors
- **Pump Control**: Output to act as the float switch on a Matelec FPC_12650
- **Additional Sensors**: Potential for soil moisture, pH, temperature, humidity, light, rain, nutrient, air quality, flow meters, wind speed and direction sensors, and cameras.

## Software Components

- **Home Assistant Integration**: Allows for real-time monitoring and automation of environmental conditions.
- **Custom Firmware**: Developed for the Leonardo R3 to handle sensor inputs and control outputs.

## Installation

### Hardware Setup

1. **Assemble the Components**:
   - Attach the DFRobot W5500 PoE Shield to the Leonardo R3.
   - Connect the DFRobot SEN0257 Gravity Water Pressure Sensors to the appropriate analog inputs on the Leonardo R3.
   - Connect the output from the Leonardo R3 to act as the float switch on the Matelec FPC_12650.

2. **Additional Sensors** (if applicable):
   - Connect additional sensors to the remaining analog or digital inputs on the Leonardo R3 as needed.

### Software Setup

1. **Clone the Repository**:
   ```sh
   git clone https://github.com/yourusername/EnviroControl.git
   cd EnviroControl
   
2. **Install Dependencies:**
Ensure you have the necessary libraries installed for the Leonardo R3 and the sensors being used.

3. **Upload the Firmware:**
Use the Arduino IDE to upload the custom firmware to the Leonardo R3.

4. **Configure Home Assistant:**

   - Add the necessary configurations to your Home Assistant setup to integrate with EnviroControl.
   - Refer to the Home Assistant documentation for integrating custom sensors and switches.
### Usage
1. **Monitor Water Levels:**

   - Use the Home Assistant interface to monitor the water levels in your tanks.
   - Automate pump control based on the water level readings.
2. **Garden Bed Monitoring (if applicable):**

   - Monitor soil moisture, pH, and other environmental factors in your garden beds.
   - Automate irrigation and other controls based on sensor readings.
3. **Real-Time Alerts and Automation:**

   - Set up real-time alerts for abnormal conditions.
   - Automate actions such as turning on/off pumps, adjusting irrigation schedules, etc.
### Future Enhancements
   - **Expand Sensor Support:** Add support for additional types of sensors as needed.
   - **Improve Home Assistant Integration:** Enhance the integration with Home Assistant for more advanced automation and monitoring capabilities.
   - **Add Documentation:** Provide detailed documentation for each component and configuration.
### License
This project is licensed under the Creative Commons Attribution-NonCommercial 4.0 International License. You can view the full license [here](https://creativecommons.org/licenses/by-nc/4.0/).

### Contributions
Contributions are welcome! Please fork the repository and submit a pull request with your improvements.

### Contact
For any questions or support, please open an issue in the repository.
