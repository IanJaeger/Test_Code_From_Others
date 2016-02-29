# Test_Code_From_Others
Borrowed code to see how things work

# for MAX6675_1
https://github.com/keiichishima/RPiSensors


# For MAX675_2
https://github.com/draco003/max31855

thermocouple.cleanup()
  
  ```
 +## MAX6675 example
 +
 +
 +```python
 +
 +#!/usr/bin/python
 +from max6675 import MAX6675, MAX6675Error
 +
 +cs_pin = 24
 +clock_pin = 23
 +data_pin = 22
 +units = "c"
 +thermocouple = MAX6675(cs_pin, clock_pin, data_pin, units)
 +print(thermocouple.get())
 +thermocouple.cleanup()
 +
 +```
 +
  
  *Note: these are the GPIO pin numbers, not the header pin numbers.*  
  *This can be overriden by passing `GPIO.BOARD` as the fifth [init parameter](https://github.com/Tuckie/max31855/blob/master/max31855.py#L11).*
