# MEE416 -- Information you may need
## Table of Contents
1. [Lab1](#lab1)

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
