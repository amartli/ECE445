# ECE445

### 02/01/2022 Project Approved
We got our idea approved


### 08/02/2022 First meeting with our TA
He gave us general information about the project such as the budget that we have, told us to do 
the proposal

### 02/09/2022 Finishing the proposal
We have finished the last parts of our proposal. I have redact the introduction, 3 level requierments,
some sybsytems requirements, tolerance analisys and some ethics points.

### 02/10/2022 First proposal uploaded
We uploaded our first version of our proposal


### 02/14/2022 Design Document Check Sign-up
We signed in for the design document check on next Tuesday (02/22/2022) at 10 a.m.


### 02/15/2022 Analysis of possible cost of out project
We realized that we are goint to exceed for sure the budget. We have 150$ of budget and our project
is going to cost approximately 350$. It ha sense because we need solar panel, large battery, precise 
sensors and uvlight. UVlight water purification systems are sold for 2000$. Our project is cheap 
compared to that.


### 02/16/2022 Second meeting wwith the TA
In this meeting he told us that:
- We only need 3 level requirements, and simplify them. Put more details in the subsytem requirements
part. Delete the last one because is the weakest
-Put othe calculations for the minimum water flow requirement in the tolerance analysis part. Write 
abut the decrease in the maximum water flow as a measure to indicate when to remplace the filter
- Put in the tolerance analysis when the manufacturer recommend changing each of the filters 
(2 and 12 months).
- Check if the battery can be charged and charge at the same time. If not, implement a switch  or some
other way to know when the user is going to use the product.
-To add components to kicad, try to add some libraries
- Do the PCB as soon as possible.


### 02/18/2022 Soldering assignment done
I spent Friday morning soldering the board and testing its operation by programming it.

Looking information to solve the problem of charging and discharging the battery at the same time.
I have found that using a blocking diode between the solar panel and the battery could solve the
problem. The problem is that our solar panel maintain the voltage constant so this solution doesnt work


### 02/19/2022 Work with Kicad
I tried to find the components that we need in kicad -> they are not included in the main library
I tried to find other libraries that contain or components -> Nothing
I tried to design the microcontrollerkit with Kicad.


### 02/20/2022
Use a solar charge controller to charge the battery and power the load at the same time. And at night
use the battery as a supply.

Check our 18/25 grade in the proposal to improve and get a better mark in the design document

Realized that we dont need to add all of our compenents to the PCB. We just need to add the
connectors.