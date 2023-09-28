# Arduino-Uno-Quadcopter
Arduino IDE code for Arduino UNO to fly a normal quadcopter drone.

This code is for flying a low budget drone (NOT FOR INDUSTRIAL PURPOSES), low powered and for beginners, powered with Arduino UNO instead of any flight controller.
Recommended build is making sure the whole weight of the drone dosent exceed 900 grams.
DC motors of 1000 kV work fine with size 10 inch propellors, also works with size 8 inches depending on your build size.
30A ESCs to be used, an Arduino UNO and an MPU for gyro sensing and caliberation.
Battery of 2200 mAh is preffered, but works with higher.
For a telemetry ( remote flight control ) a flysky works perfectly.


If the drone dosent fly properly, these might be some of the things you could try:
- checking all the connections from the ESCs, the flight controller and the Arduino.
- checking if the propellors are connected properly making sure the CCW and CW propellors are fixed on their respective DC motors and not the opposite.
- make sure the DC motors are fixed on the proper arms, the rule is to have two opposite rotating motors adjascent.


Run the "eeprom" code first to clear the EEPROM data from the Arduino ( not essential but considered a good practice )
Run the "setup" code next and follow the instructions that pop up in the serial monitor.
Run the "calibrate" code next and after the sketch is done compiling and uploading, type "r" in the serial monitor and press enter, then change the thust sloely using the telemetry to get the various Start 0-1-2 values, then type "a" in the serial monitor and press enter. After doing the same unplug thr Arduino from the device you are coding in.
after closing all the previous codes, test if all the motors are functioning properly with the thrust.
Finally run the "flight" code and disconnect the arduino board again.


Conduct a test flight and recalibrate if any issue arises later, or change the initial values in the code if you know what you are doing.
