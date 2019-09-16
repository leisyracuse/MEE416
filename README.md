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
- machine extention from preload: the istance that load cell moved after pre-load
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
The equation given in lecture slide and student lab manual is for **fixed-fixed** boundary condition. Our test is **pinned-pinned** condition. You can search online to find the correct equation.
