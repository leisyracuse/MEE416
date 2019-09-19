# MEE416 -- Information you may need
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
### 9. Uncertainty
![](https://blackboard.syracuse.edu/webapps/blackboard/content/listContentEditable.jsp?content_id=_5055164_1&course_id=_388813_1&mode=reset)
