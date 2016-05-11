# MPU6050_vpython
This contains a project involving Dual MPU6050 in the same I2c Bus (used GY521 breakout board).
The project was intended for getting the motion of Human arm by wearing these tiny sensors.
One of the MPUs must have AD0 pin shorted to Vcc to change address to 0x69,
the Gnd must be shorted to AD0 in the other MPU6050,its address becomes 0x68.
  ARDUINO:

    The arduino program gives an array of 6 values roll ,pitch ,yaw angles of each sensor in degrees.
  
  PYTHON:
    The Vpython code recieves these from the serial port, and shows a stick model animation of the arms moving.
    The initial values and orientation of these sensors should be changed in the python program for better results.
