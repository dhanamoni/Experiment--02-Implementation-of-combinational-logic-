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
## Program:
~~~
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
Developed by: Monika D
RegisterNumber: 23013746  
~~~
## RTL realization
![Screenshot 2023-12-13 015932](https://github.com/dhanamoni/Experiment--02-Implementation-of-combinational-logic-/assets/151629757/a8889092-7127-48f7-a975-1c8e2b1c0c44)

## Truth table:
![Screenshot 2023-12-13 020200](https://github.com/dhanamoni/Experiment--02-Implementation-of-combinational-logic-/assets/151629757/ceb8947f-1752-44db-b075-3de7e035e6af)

## Timing diagram
![Screenshot 2023-12-13 020333](https://github.com/dhanamoni/Experiment--02-Implementation-of-combinational-logic-/assets/151629757/b612e59e-3817-4cc1-a19a-6538a62eccd1)

## Result:
Thus the given logic functions are implemented using  and their operations are verified using Verilog programming.
