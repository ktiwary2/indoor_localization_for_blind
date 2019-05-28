# indoor_localization_for_blind

For our senior design project, we built wrist wearable devices that would provide indoor navigation to
blind people. They function through Bluetooth communication with strategically positioned Bluetooth
beacons across the characterized apartment. In order to give the best experience, we have developed user
localization and path planning features in order to guide users to their final destinations. 

On the hardware side, the user can pick his/her destination through touch and will receive haptic feedback for navigation.
The testing and characterization was done in a team member's apartment (see maps attached). Ultimately, we got each of our
modules working with successful Bluetooth communication and proper input/output interaction.

A Particle Filter is used for the localization module (code given in Github). The Environment Characterization
is important to develop the measurment model for the localizatoin. Gaussian Process Regression was
finally used. Training data consisted of RSSI values from each of the four beacons at every point in the 
apartment using the reciever module. 

We did run into some memory computation problems, as the localization was done through a
Particle filter, which required an immense amount of dynamic memory from the microprocessor.