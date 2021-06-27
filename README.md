# floor_cleaner_bot
The pins have to be connecting as per the following:
•	Signal 1 ---- D6 on Arduino
•	Signal 2 ---- D9 on Arduino
•	Signal 3 ---- D10 on Arduino
•	Signal 4 ---- D11 on Arduino
•	+5V ---- +5V on Arduino
•	Gnd ---- Gnd on Arduino
•	+12V (motors will move at this voltage) ---- to be connected to battery later
Then for the bluetooth module. Connections are like:
•	Vcc ---- +5V on Arduino
•	Gnd ---- Gnd on Arduino
•	Rx ---- Tx on Arduino
•	Tx ---- Rx on Arduino
	The two mop motors have to be connected in parallel such that the left one runs anticlockwise and the right one turns clockwise when seen from the front. Use heat shrink tubes to keep the connections safe. Solder the motor wires to the transistor circuit as per the schematic given above. Similarly connect the water pump wires as well.
	We will be supplying the 12V from the battery directly to the transistor circuit and then this 12V will go to the Vcc of arduino and the motor driver circuit.
	Connect the base of transistor two, controlling the mops to D5 on arduino and transistor one, controlling the pump to D4 on arduino. The common ground wire from all the motors has to be connected to the Gnd on arduino.
	What remains now is the servo motor. The connections are:
•	Vcc ---- +5V on Arduino
•	Gnd ---- Gnd on Arduino
•	Signal ---- D3 on Arduino
	Next, take two straws, Crush and squeeze one end of both into the outlet pipe of the water pump. Bend both of them in opposite directions and glue them in place such that water flows from both the straws and falls just a little ahead of the rotating mop. 
	Final step is to upload the code in arduino UNO
	We removed the Rx and Tx cables from arduino before uploading.
