# Hand-Gesture-Controlled-Car
# Project finished September 2022
# Github created December 4th 2023
Arduino based project where a car has its movement controlled by different hand positioning.

The Car:

An arduino connected to a car chassis with 4 wheels that connect to an Adafruit motor shield v2. The car received commands from a HC-05 bluetooth module.

- The motor shield allowed easy control of the motors without damaging the arduino or any other components. Due to its size, the motor shield also kept the car module compact in size

- The (child) bluetooth module took a certain command such as 'f' for forward or 'b' for backward, and turned it into lines of execution that the motor shield could use to drive movement.

-----------------------------------------------------------------------------------------------------

The Controller:

Arduino nano with makeshift glove that took values from an MPU-6050 gyroscope and accelerometer and sent them to the car via a HC-05 bluetooth module.

- The gyroscope/accelerometer measure the tilt and angle positioning of the hand to determine what information to give to the controller's bluetooth module

- The (parent) bluetooth module received information about the orientation of the MPU-6050, and sent commands to the child bluetooth module based on that information


