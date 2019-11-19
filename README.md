# MEE416 -- Information you may need
## Table of Contents
1. [Lab1 Solid Mechanics](#lab1-solid-mechanics)
2. [Lab2 Heat Transfer](#lab2-heat-transfer)
3. [Lab3 Linear Control](#lab3-linear-control)
4. [Lab4 HVAC](#lab4-hvac)

## Lab1 Solid Mechanics
### 1. Power supply to wheat stone bridge
Input voltage is 8V 
### 2. Coefficient of strain gauge
k = 1.77
### 3. Structure of raw data
#### 3.1 Bending
- load: the force added by loading cell
- machine extention: the distance that load cell moved during the test
- machine extention from preload: the distance that load cell moved after pre-load
#### 3.2 Buckling
- load: the force added by loading cell
- machine extention: transverse deflection
- crosshead: the distance that load cell moved during the test (axial displacement)
### 4. Length of test sample (Buckling)
length of all the test sample (steel, aluminum, carbon fiber) are 1 ft
### 5. Import raw data to Matlab
There are some ways to import test data into Matlab. You may have a very specific issue, so I can not answer everyone's question here.
The simpliest way is copy the data in txt file to excel. Then on the "**Home**" tab, in the "**Variable**" section, select "**Import Data**" in Matlab.  
For more information https://www.mathworks.com/help/matlab/data-import-and-export.html
### 6. Critical load calculation
The equation given in lecture slide and student lab manual is for **fixed-fixed** boundary condition. Our test is **pinned-pinned** condition. The equation of **pinned-pinned** shows below:  
![](https://latex.codecogs.com/gif.latex?P_%7Bcr%7D%20%3D%20%5Cfrac%7B%5Cpi%5E2EI%7D%7BL%5E2%7D)

### 7. Plot of theoretical relationship between strain and stress for bending test
In order to plot the theoretical relationship between strain and stress for bending test, a theoretical Young's Modulus (E) for steel (E=200Gpa) can be used. 
### 8. Theoretical coefficients for buckling test.
|   |Aluminum|Steel|Carbon Fiber|
|---|---|---|---|
|Young's Modulus (E) [Gpa]|77|200|70|
|Yield stress [psi]|35000|54000|75000|
### 9. Uncertainty and Resolution
#### LS5 Technical specification
![LS5](https://github.com/leisyracuse/MEE416/blob/master/Technical%20Specification.png)
#### Deflectometer
![Deflectometer](https://github.com/leisyracuse/MEE416/blob/master/Deflectometer.png)
#### Calipers
Ordinary 6-in/150-mm digital calipers are made of stainless steel, have a rated accuracy of 0.001 in(0.02mm) and a resolution of 0.0005 in (0.01 mm)
#### The time component of the testing machine
It is the resolution of the computer clock. Less than 100ns.
#### Strain gage
![strain gage](https://github.com/leisyracuse/MEE416/blob/master/sg.jpeg)
#### Bridge completion module
![bridge completion module](https://github.com/leisyracuse/MEE416/blob/master/Bridge%20Completion%20Module.jpeg)

## Lab2 Heat Transfer
### 1. Clarification and Correction
1. Student manual Page11 Appendix1, Thermal conductivity of Fin surface is 205 W/(m*K)
### 2. Dimensions of fins
![fin1](https://github.com/leisyracuse/MEE416/blob/master/Fins.PNG)
![fin2](https://github.com/leisyracuse/MEE416/blob/master/Fins2.PNG)
### 3. Perimeter and Cross-section Area
* Perimeter and area in Page 11 Appendix 1
  * "Perimeter" is the perimeter of __section B-B__
  * "Cross area" is the __surface area__ of a single fin exposured to ambient air
  * "Total area" is the surface area of single fin __times 9__ (we have 9 fins on the heat sink)
* Perimeter and cross-section area in Eq 3-65
  * "Perimeter" is the perimeter of __section A-A__
  * "Cross-section area, Ac" is the cross-section area of __section A-A__
 
Three view drawing of a single fin:
![single fin](https://github.com/leisyracuse/MEE416/blob/master/singleFin.png)

## Lab3 Linear Control
### 1. Uncertainty and Resolution
There is no avaiable information about instrument specification for this lab.

## Lab4 HVAC
### 1. Cross dimension of air duct
155mm * 155mm
### 2. Calculation of removed sensible heat, latent heat and moisture
After you plot point 1 and 2 for two different states, just project these two points perpendicular to the bottom axis (temperature) and the right axis (humidity ratio), then you'll find an intersection point 3. Project point 1, 2 and 3 to the enthalpy axis, you can get the enthalpy for these three points. The enthalpy difference between point 1 and 2 is the total enthalpy difference, the enthalpy difference between point 3 and 2 is the sensible enthalpy difference and the enthalpy difference between point 1 and 3 is the latent enthalpy difference. By multiplying the enthalpy difference and the air mass flow rate, you can get either removed total, sensible or latent heat. From the humidity ratio difference between point 1 and 2, you can get the removed moisture (by multiplying with the air mass flow rate). The equations are: 

**Total heat removed:** q_t = m * (i1 - i2)

**Sensible heat removed:** q_s = m * (i3 - i2)

**Latent heat removed:** q_l = m * (i1 - i3)

**Moisture removed:** m_w = m * (W1 - W2)

*q_t: total heat removed*

*q_s: sensible heat removed*

*q_l: latent heat removed*

*m: mass flow rate of air*

*i: enthalpy*

*m_w: moisture removed*

*W: humidity ratio of air*

![psychrometric chart](https://github.com/leisyracuse/MEE416/blob/master/psychart.PNG)
