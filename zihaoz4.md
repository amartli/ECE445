# ECE445
### 01/28/2022 Start discussing potential topics
Including Alcoholic analyzer and tilt detector for vehicle secured ignition, Auto guided vehicle with material handling and obstacles detection, Automatic plant watering and tank level alerting system

### 01/30/2022 Fixed the idea as the filter with uv light disinfection
This topic appeared to be the most reasonable and practical one.

### 01/31/2022 Project Approved

### 02/02/2022 information gathering started
Split topics included solar panel, water flow sensor, microcontroller, uv light, and search information about the products on the market.

### 02/07/2022 detailed meeting with the construction of whole project
We assembled the components we chose to build the concept construction of the project. I recorded the block diagram as needed.

### 02/08/2022 Modify the design
We were keeping modifying the design and the block diagram based on the products we could buy. We discussed about the details including how to protect the user from the uv light.

### 02/09/2022 Visual aid
We prepared the visual aid to show the machine shop and get feedbacks.

### 02/10/2022 parts selection
Try to build the circuit requirements based on the parameters of the components such as sensors and microcontrollers we are going to buy.

### 02/15/2022 flow rate sensor discussion
We find out that most of the flow sensors are having a high minimum detection rate comparing to the rate of water being filtered theoretically by our filters. We tried to think of another way to solve the problem but we still think that a flow sensor is the best solution. I created the draft of the circuit which would be used to build the pcb.

### 02/16/2022 battery discussion
We found out that the battery can not be charged and act as a power source at the same time, which means that we need a way to control the time when the battery is being charged and when the battery should supply power.

### 02/20/2022 charge controller
We find out that a charge controller can solve the problem of the battery which means it can automatically stop the charging of the battery when parts are drawing power from it. 
### 02/21/2022 design document preparation
We tried to finalize the design document and keep modifying block diagram, parts selection to lower the total cost.

### 02/22/2022 design document check
Receive suggestions from the professor and TAs, made modifications to the system including removing unreasonable suggestions and add pre filters. Finalized the concept of the reason to change the filters: ”avoid user to waste time”. We debated about whether to add the activated carbon filter and how we can control the replacement of it. We decided to use it and use the record of amount of water going through the filter to determine when to replace it.

### 02/24/2022 design document finalization
After communication with the machine shop and the professor, we finished the design document. 

### 02/27/2022 pcb design start
After Alberto created the draft of the circuit design, I started to search the way of adding components not included in the library to the circuit and do footprint to create the pcb design.

### 02/28/2022 RLC selection
Computed the theoretical power, current and voltage of each component in the circuit to decide the values of the RLCs. Decided to use Mosfet to control the on/off of the LEDs.

### 03/01/2022 Design Review presentation
Discussed more about the voltages and the RLCs. Vcc of most components should be 5V. voltage of the two uv lights should be 5.7V to provide enough power to disinfect the water in a reasonable amount of time. Find it hard to do water quality detection especially for the heavy metal content.

### 03/05/2022 buying parts and pcb design
Select the jumpers to connect the uv light, water sensor and water flow sensor, ISP for programming cable, voltage source from the charge controller. Keep modifying the circuit diagram and the pcb design.

### 03/06/2022 modifying pcb design and buy filtering parts
Decided the dimensions of the RLCs and other parts. Check the dimensions and parameters of every component. We bought the filters and the tank, with pre filter. 

### 03/08/2022 finalizing pcb design
I finalized the design of the pcb and passed the audit. 

### 03/10/2022 machine shop meeting
Talked with the machine shop to make sure what they can do for us. They said that the uv lights can not be placed inside of the lower tank because it is hard to make it waterproof. The tank would not block the uv light so we put them under the lower tank.

### 03/21/2022 machine shop check
Check the project the machine shop made for us. The biggest problem is that the activated carbon filter is not working due to the height of the upper tank cannot provide enough water pressure to surpass the tight construction of the filter. We decide to give up the second filter for the testing but still include it as theoretical design.

### 03/24/2022 machine shop conflict
Machine shop’s core value is that we are just making a prototype rather than a mature commercial product so they won’t care about user friendliness. For the lid they are not going to add because that is meaningless. The pre filter is glued on the iron sheet which placed on the top and they can only be removed together to be cleaned. We are supposed to add water before the water level reaches the connector point on the water detector so no protection or change on the water detector they would make. They think that amount of water is enough for us to do experiment. The first filter is fixed on the black box, if we need to replace it we need to take the screws out and black box out. The reason why the flow rate is low and the carbon filter is not working is probably because the water level for our design is too low to create enough water pressure comparing to the one designed by lifestraw. To summarize, we are not getting any modifications upon on the picture they sent to us yesterday. I gave them the solar panel to let them fix it on the side and that’s basically what all they can do for us.

### 03/30/2022 Shipment delay
After we have been waiting for several days, we asked about why our things have not been delivered by emailing mouser. They said that our shipment has been delayed and they are trying to ship it again. The 5v converter is also out of stock so we need to buy it again with battery and microcontroller. We find that the diodes we bought were too tiny which was impossible for us to directly solder them. 

### 04/01/2022 water verification cancel
The labs available are not able to test virus of the water being filtered. After discussed with the professor we decided not to do the verification of the quality of the water being filtered by the filters. 

### 04/04/2022 diode soldering
I added external wires to the pcb in order to adapt larger diodes. It was too tiny but I made it finally.

### 04/05/2022 Microcontroller soldering
I have done soldering the microcontroller, and checked that every used pin is connected to the board. 

### 04/07/2022 solar panel connection problem
Find that the solar panel can not be directly connected to the charge controller. Buy another jumper. Also, the connector wire of the water flow detector does not match the header on the pcb. Cut the wires and get external connections. 

### 04/09/2022 Testing and burning of the converter
We roughly completed the connection and tried to test if we can get the voltages we want. However, when we connected the 4.2V which is the Vout from the charge controller, the 5V boost converter directly burns. We finally find out that the reason is that we bought a wrong one in the second shipment which was designed for Vin to be 2V while 4.2V is too large for it. We bought all the components again just as backup to avoid further similar destruction and possible delay.

### 04/13/2022 Unusable chip programming
We found that although we have the draft code for our project, we can not find application to program it from the computer to the microcontroller. It is too old which can not be programmed by computer system today. 

### 04/16/2022 New chip ordering
We ordered another chip and we are trying to connect it by wires just as we did for the diodes. 

### 04/18/2022 new pcb design
We found that it is impossible to connect the new chip to the board through wires, so we decide to buy another pcb with new connections. 

### 04/19/2022 circuit modification
We find that the new 5V boost converter(after burning) was not working with the old RLC and diode connection. Therefore, when design the new pcb we need to follow the new suggested connection in the datasheet. 

### 04/20/2022 new pcb ordering
I complete the design of the new pcb with new 5V converter circuit and microcontroller connection, and buy the new pcb through pcbway. We expect to get it on 4/25, Monday. 

### 04/22/2022 breadboard building
We build our pcb on a breadboard for testing. The 5V and the 7V boost converter are working fine this time. 

### 04/23/2022 pcb delay
Due to problem of shipment between China and United States these days the pcbs are not arriving on time. We are trying to make the breadboard working. 

### 04/24/2022 new chip failure
The bootloader can not be burned for the new chip. What we could do was just checking the connections of the whole breadboard are working. We are going to solve the microcontroller problem in office hour on Monday.

### 04/25/2022 chip switching and water flow sensor shorting
After asking the TA we tried to add an external oscillator to our circuit to see if the new microcontroller can be working. The result is negative. We finally decide to use the ATmega 48 as our final chip. Still working on the circuit to add external LEDs to unit test the microcontroller states. We didn’t limit the current supply one time so it gets to 200 mA when the maximum current going through the water flow sensor is 25mA. We put voltmeter between the signal node and the ground node and we found them to be connected which means a short is between them and the flow sensor is destroyed(even bad smell come out of it).

### 04/26/2022 Finalizing project for demo
We work the whole day to finalize the project. We spent most of the time trying to figure out the way to tell when the user should change the filter without the water flow sensor working. We found out we can use the water sensor in the upper tank to do this. Under normal water flow, the time taken for water level to drop from the upper line of the water sensor to the bottom of it is approximately 25 minutes, so as we are setting half flow rate as the criteria for the user to change the filter, if the water sensor is detecting water to stay on it for more than 50 minutes, the indicator should light up. We set this logic in our new program and get it to work finally. 

### 04/28/2022 Presentation preparing
We take pictures and record videos for all the successes and failures. We made the slides for the presentation. 

### 04/29/2022 Presentation feedback
Eye contact, too many slides, more results than theoretical thoughts. Add flow chart. Shorting RV table. Label photos. 

### 04/30/2022 Final works
Start to write the final paper and keep modifying the slides.

