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
/*
Program to implement the given logic function and to verify its operations in quartus using Verilog programming.

Developed by: Revanth Palagiri
RegisterNumber:23002622

program:module logic(a,b,c,d,w,x,y,z,F1,F2);
input a,b,c,d,w,x,y,z;
output F1,F2;
wire A1,A2,A3,A4,A5,B1,B2,B3,B,B5;
assign A1=(~a&(~b)&(~c)&(~d));
assign A2=(a&c&(~d));
assign A3=((~b)&c&(~d));
assign A4=(~a&b&c&d);
assign A5=(b&(~c)&d);
assign F1=A1|A2|A3|A4|A5;
assign B1=(x&(~y)&z);
assign B2=(~x&(~y)&z);
assign B3=(~w&x&y);
assign B4=(w&(~x)&y);
assign B5=(w&y&z);
assign F2=B1|B2|B3|B4|B5;
endmodule
*/
## RTL realization

## Output:
## RTL:
![Screenshot 2024-01-02 204009](https://github.com/Revanth-2717/Experiment--02-Implementation-of-combinational-logic-/assets/152462274/4a74625c-774d-45a9-ab5e-5f7b2bea9e72)
Truth table:
![Image 2024-01-02 at 20 39 24_6a26fb22](https://github.com/Revanth-2717/Experiment--02-Implementation-of-combinational-logic-/assets/152462274/ed1a9ac9-6dbc-4d4f-9134-0748f9f297cf)

## Timing Diagram:
![Image 2024-01-02 at 20 39 24_b25f88da](https://github.com/Revanth-2717/Experiment--02-Implementation-of-combinational-logic-/assets/152462274/ff69d2da-0b0e-43a4-be1c-8d66abc96fcb)

## Result:
Thus the given logic functions are implemented using  and their operations are verified using Verilog programming.
