* c1500_light_switch
Intelligent light switch for Chevrolet C1500 head light switch. 
** Reasoning
** Requirements
Below are the following requirements that the light switch unit shall meet.
*** Mechanical
**** A housing shall be developed to house the electronics in the original light switch location. 
**** The design for the unit shall be developed in FreeCAD. 
**** The unit shall be capable of being printed with a commodity fused deposition modeling printer (aka 3D printer).
**** The unit shall fit within the same area that the OE unit was in.
**** The unit shall utilize the original securing plastic features that the OE unit was in. 
**** The unit shall provide reasonable protection from exposure to live circuits. 
*** User Interface
**** The unit shall utilize capacitive sensing for accepting user intent to toggle lights.
**** The unit shall provide at least 3 buttons for the user to indicate the following commands.
+ All lights off
+ Parking lights on
+ Headlights + Parking lights on
*** Electrical
**** The unit shall be powered from the provided nominal 12-14V of the vehicle.
**** The unit shall provided a means of updating the software controlling the system.
**** The until shall not impose excess drain on the vehicle battery.
***** The unit shall not draw more than 10mA when the vehicle is off and the lights are powered off.
***** The unit should not draw more than 100uA when the vehicle is off and the lights are powered off.
***** The unit shall not draw more than 100uA when the vehicle is off, not cranking, and the vehicle battery is below 12.0V.
**** The unit should provide the following operation modes
+ Daytime running parking lights
+ Engine start/stop detection
+ Headlight power off timer
+ Ambient light controlled automatic lighting. 
**** The unit should provide a means of command and status via Bluetooth Low Energy (BLE). 
***** The physical controls should be made available via BLE.
***** The status of the lights should be made available via BLE.
***** The battery voltage should be made available via BLE.
***** The power off timer should be configurable via BLE.
***** The ambient light controlled automatic lighting should be configurable vie BLE. 
** Implementation
*** Mechanical
*** Electrical
The design is controlled by a Cypress PSoC BLE module. 
**** Prospective micro-controllers
+ Cypress [[http://www.cypress.com/part/cy8c4128fni-bl583t][CY8C4128FNI-BL583T]]
+ Cypress [[http://www.cypress.com/documentation/datasheets/cyble-214015-01-ez-ble-psoc-bt-42-module][CYBLE-214015-01 EZ-BLE]]

