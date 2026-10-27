# Bhoonidhi
An Intelligent System to Protect River Yamuna and Other Holy Rivers of India.

This system uses an Unmanned Aerial System based Thermal Camera to Effectively Identify and monitor the mixing of Industrial Effluents in the rivers.

This system mainly focuses on to protect the environment of the nation and ensure good health to the its peoples and also aquatic lifes under water.

The Prototype Model Comprises of Two Modules,
They are,
  1) Unmanned Aerial System Module.
  2) Thermal Camera Module.

Module 1: Unmanned Aerial System
Components Required:
Receiver:
  1) 720 Motors- 2 Clockwise and 2 anticlockwise.
  2) 40mm Propeller - 4 pcs
  3) Battery > 25C
  4)  XIAO ESP32 S3
  5)  MPU 6050 Gyroscope Sensor
  6)  AO3400A Mosfet
  7)  0805 10k Resistor
  8)  B5819 Schottky Diode
  9)  30AWG Wires.
Transmitter:
  1) Two Joystick Module
  2) ESP32 Microcontroller
  3) 4 Buttons
  4) 18650 Battery
  5) XL6009E1 Booster

Setup:
 1)Pairing the gyroscope 
 
 
 <img width="187" height="104" alt="image" src="https://github.com/user-attachments/assets/70c32240-b54d-423f-b3c7-ecc40d3ab0f7" /> 
 
 We are using betaflight-configurator_10.10.0_win64-installer.exe to install the BetaFlight and then setting up the Firmware.

 2)Configuring the Software in the BetaFlight
  PID loop frequency - 2.000 kHz
  Motor protocol- BRUSHED
  Motor PWM frequency- 8000

  3) Motor Driver assembly
    
    
  <img width="184" height="191" alt="image" src="https://github.com/user-attachments/assets/53d7b6cc-513e-4b68-9507-0e2a7734a113" />

  4)Wiring the System 
  
  
  <img width="293" height="259" alt="image" src="https://github.com/user-attachments/assets/4c5ea47d-67fe-409c-a0b3-ec280fb11555" />

  5) Testing and Flight
     Check the working of each motors in the BetaFlight by powering up one after another, we are ready to go with the flight.

Module 2: Thermal Camera

MIO802 Thermal Camera Module Specifications:  
Sensor Type- LWIR hybrid CMOS-compatible SenXor TM Technology
Resolution: 4960 pixels
Output- Radiometric
Shutter- Shutterless
Frame Rate- up to 29.3 FPS
Power Supply- 3. V
SPI Clock- 10-20 MHz
Module Weight- <30 grams

Network and Software Setup:
1)The ESP32 Thermal Camera and the microcontroller has to be connected in the same wifi network.
2) The Wi-Fi Router enable to thermal camera to act as a TCP Server and microcontroller acts as TCP Client.
3)The connection establishment takes between between TCP Client and TCP Server.
3) Once connection is established the tansfer data between the TCP Client and TCP Server takes place.
4) The microcontroller identifes the Change in the Temperature and immediately send the alerts.

By this way, the mixing of Industrial Effluents in the Rivers can be effectively identified and monitored continously.






 

 
 


