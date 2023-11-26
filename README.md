# Experiment--02-Implementation-of-combinational-logic
Implementation of combinational logic gates
 
## AIM:
To implement the given logic function verify its operation in Quartus using Verilog programming.
 F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D
F2=xy’z+x’y’z+w’xy+wx’y+wxy
 
 
 
## Equipments Required:
## Hardware – PCs, Cyclone II , USB flasher
## Software – Quartus prime


## Theory
 

## Logic Diagram
## Procedure

Program to implement the given logic function and to verify its operations in quartus using Verilog programming.
Developed by: MADHANRAJ P
RegisterNumber:  23013616
## CODE:
module ex_02(a,b,c,d,f1);
input a,b,c,d;
output f1;
wire x1,x2,x3,x4,x5;
assign x1=(~a)&(~b)&(~c)&(~d);
assign x2=(a) &(~c)&(~d);
assign x3=(~b)& (c) &(~d);
assign x4=(~a)& (b) & (c) & (d);
assign x5=(b) & (~c)&(d);
assign f1=x1|x2|x3|x4|x5;
endmodule
## RTL realization:
![image](https://github.com/madhanraj67/Experiment--02-Implementation-of-combinational-logic-/assets/150319515/cbc98fc9-c4f0-4da4-8f15-1666b67d240e)
## TRUTH TABLE:
![image](https://github.com/madhanraj67/Experiment--02-Implementation-of-combinational-logic-/assets/150319515/be2b6134-b79e-48be-bfa6-549f31663090)

## OUTPUT:
![image](https://github.com/madhanraj67/Experiment--02-Implementation-of-combinational-logic-/assets/150319515/7f4ba72a-4705-47dd-8503-7e085c0dcc20)

## Result:
Thus the given logic functions are implemented using  and their operations are verified using Verilog programming.
