# Automatic electronic on-off circuit design 

With this design, I can entirely turn off the power while the Arduino is not in use.
So to do that I wrote the working method on several steps.
- The Arduino receives power when I press the circuit's pushbutton. The Arduino then starts up.
- To keep the circuit switched on, I set the LATCH pin to HIGH.
- Tasks are carried out by the Arduino. In my example, it only uses a photosensor to detect light, assess brightness, and turn on an LED if the brightness level is low.
- To enable auto-shutdown of the Arduino, I set the LATCH pin to LOW.
- Power is turned off when the LATCH pin is set to LOW.
