# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**

**Logic Diagram**

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**
~~~
module EXP2(
input a,b,c,d,
input w,x,y,z,
output f1,f2
);
assign f1=(~b&~d)|(a&b&~c)|(~a&b&d);
assign f2=(~y&z)|(x&y)|(w&y) ;
endmodule
~~~
/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by:KAVINKUMAR R
RegisterNumber:25002358


**RTL realization**
<img width="1920" height="1080" alt="Screenshot (54)" src="https://github.com/user-attachments/assets/0b74f5d8-0ee3-42fa-ae91-1b74e316a321" />


**Output:**

**RTL**
<img width="1386" height="738" alt="Screenshot 2025-11-22 080417" src="https://github.com/user-attachments/assets/ef9e1c37-552c-4227-b3a2-7ab069a48e9b" />


**Timing Diagram**

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

