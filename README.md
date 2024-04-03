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

 Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by: THILAKESWARAN

RegisterNumber: 212223230232
```py
module combinationalcircuit(A,B,C,D,F1);
input A,B,C,D;
output F1;
wire x1,x2,x3,x4,x5;
assign x1=(~A)&(~B)&(~C)&(~D);
assign x2=(A)&(~C)&(~D);
assign x3=(~B)&(C)&(~D);
assign x4=(~A)&(B)&(C)&(D);
assign x5=(B)&(~C)&(D);
assign F1=x1|x2|x3|x4|x5;
endmodule
```
**RTL realization**

![image](https://github.com/Gokhulraj2005/BOOLEAN_FUNCTION_MINIMIZATION/assets/138849253/31abede3-4039-4e7f-af3d-3812d4056efc)


**Timetable**
![image](https://github.com/Gokhulraj2005/BOOLEAN_FUNCTION_MINIMIZATION/assets/138849253/0dd80e62-e167-40fc-862e-ff155741ea45)



**Timing Diagram**

![image](https://github.com/Gokhulraj2005/BOOLEAN_FUNCTION_MINIMIZATION/assets/138849253/9924e9e4-612d-4ea6-85f7-46c07639c48a)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

