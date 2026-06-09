# Mean-and-variance

EXPT.NO.8	SIMULATION OF MEAN AND VARIANCE USING SCILAB

AIM:
To write a program for mean, variance and cross correlation in SCILAB and verify the output.

EQUIPMENTS Needed

•	Computer with i3 Processor
•	SCI LAB

Algorithm
1.	Define	the	Function:	Specify the	function	you	want	to	simulate.	For	example, f(x)=sin⁡(x)f(x) = \sin(x)f(x)=sin(x) or any other function.
2.	Generate Sample Points: Decide on the range and the number of sample points. Generate these sample points within the desired range.
3.	Evaluate the Function: Compute the function values at each of these sample points.
4.	Compute Mean, Variance and Cross Correlation: Use Scilab's functions to calculate the mean and variance of the computed function values.
5.	Display Results: Output the computed mean variance and Cross Correlation

   PROCEDURE
•	Refer Algorithms and write code for the experiment.

•	Open SCILAB in System

•	Type your code in New Editor

•	Save the file

•	Execute the code

•	If any Error, correct it in code and execute again

•	Verify the generated results

PROGRAM:
```

function X=f(x) 
    z=3*(1-x)**2; 
    X=3*x*z; 
endfunction 

a=0; b=1; 
EX=intg(a,b,f); 
disp(EX,"i) Mean of X =") 


function X2=g(x) 
    z=3*(1-x)**2; 
    X2=3*x**2 *z; 
endfunction 

EX2=intg(a,b,g); 
vX=EX2-(EX)**2; 
disp(vX,"ii) Variance of X ="); 

x=[1 2 3 4 4 3 2 1]; 
n=max(size(x))-1; 

r=corr(x, n+1); 

plot2d3('gnn', r);


```
TABULATION
<img width="1204" height="1600" alt="image" src="https://github.com/user-attachments/assets/18f4be52-4a11-4529-a377-e5072258f501" />


CALCULATION

1.Mean of X=2
2.Variance of x:-0.8
<img width="1048" height="1600" alt="image" src="https://github.com/user-attachments/assets/6e65c15b-5dc1-44e0-8096-3df831df907f" />
<img width="1536" height="1378" alt="image" src="https://github.com/user-attachments/assets/7488f59b-d7fb-428a-8eba-720f443741af" />


Cross correlation
Type in the reference sequence =[1 2 3 4 4 3 2 1]


OUTPUT 
<img width="1600" height="857" alt="image" src="https://github.com/user-attachments/assets/c439739e-eddc-4566-91f3-b8fb22f9beec" />
<img width="1600" height="1368" alt="image" src="https://github.com/user-attachments/assets/b87c8ed0-2534-4621-812b-96997cc5b535" />


RESULT: 
Thus, the mean, variance and cross correlation are executed in Scilab and output is verified.



