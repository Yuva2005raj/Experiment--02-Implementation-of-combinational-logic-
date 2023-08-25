# Experiment--02-Implementation-of-combinational-logic
Implementation of combinational logic gates
 
## AIM:
To implement the given logic function verify its operation in Quartus using Verilog programming.
 F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D
F2=xy’z+x’y’z+w’xy+wx’y+wxy
 
 
 
## Equipments Required:
 Hardware – PCs, Cyclone II , USB flasher
 Software – Quartus prime


## Theory
Logic gates are electronic circuits which perform logical functions on one or more inputs to produce one output.
#### OR Gate:
The OR gate is a fundamental digital logic gate that operates on two binary inputs, producing an output of 1 if at least one input is 1. It symbolizes logical disjunction and is essential in building logical circuits and decision-making processes in computers and electronics.
#### AND Gate:
The AND gate is a fundamental digital logic gate with two inputs and one output. It produces a high output (1) only when both input signals are high (1). If any input is low (0), the output remains low. It's a building block for more complex logic circuits and is integral in digital computations.
#### NOT Gate:
The NOT gate is a fundamental digital logic gate. It has a single input and a single output. The output is the inverse of the input: if the input is high (1), the output is low (0), and vice versa. It's a basic building block in digital circuits, used for logic inversion.
 
## Procedure
1.Create a project with required entities.
2.Create a module along with respective file name.
3.Run the respective programs for the given boolean equations.
4.Run the module and get the respective RTL outputs.
5.Create university program(VWF) for getting timing diagram. 
6.Give the respective inputs for timing diagram and obtain the results.
## Program:

/*
Program to implement the given logic function and to verify its operations in quartus using Verilog programming.

Developed by: YUVARAJ B

RegisterNumber:  212222230182
```
module expression (A,B,C,D,F1);
input A,B,C,D;
output F1;
wire x1,x2,x3,x4,x5;
assign x1 = (~A)&(~B)&(~C)&(~D);
assign x2 = (A)&(~C)&(~D);
assign x3 = (~B)&(C)&(~D);
assign x4 = (~A)&(B)&(C)&(D);
assign x5 = (B)&(~C)&(D);
assign F1=x1|x2|x3|x4|x5;
endmodule
```

*/
## RTL realization
![image](https://github.com/Yuva2005raj/Experiment--02-Implementation-of-combinational-logic-/assets/118343998/ca68ab15-4ebc-42e4-a8a9-f0b88898b14a)


## Output:
![263164034-0f5eaa4c-cd5f-4454-9f48-2f455a09016f](https://github.com/Yuva2005raj/Experiment--02-Implementation-of-combinational-logic-/assets/118343998/7b24851a-fbb0-4127-a2a9-f4009c203da7)


## Timing Diagram
![263164068-b48e5329-b838-4d76-ba40-ebe2a16d24d4](https://github.com/Yuva2005raj/Experiment--02-Implementation-of-combinational-logic-/assets/118343998/027008da-1b6c-48dd-80f9-5df30f69f6e0)

## Result:
Thus the given logic functions are implemented using  and their operations are verified using Verilog programming.
