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
<img width="914" height="1600" alt="image" src="https://github.com/user-attachments/assets/97fc4492-3ffb-43c8-b951-195913848a3c" />
<img width="1582" height="1600" alt="image" src="https://github.com/user-attachments/assets/d7752f7c-8610-4fbc-84e0-a9ccffd1b22c" />

CALCULATION

1.Mean of X=0.75
 

2.Variance of x:-0.2625
  

Cross correlation
Type in the reference sequence =[1 2 3 4 4 3 2 1]


OUTPUT 
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/06321cef-da0c-4332-99c2-264c0fcd763a" />

RESULT: 
Thus, the mean, variance and cross correlation are executed in Scilab and output is verified.



