## NAME:Pavithra.S
## REGISTER NUMBER:212223230147
## Experiment--04-Half-Subtractor-and-Full-subtractor
## AIM:
To design a half subtractor and full subtractor circuit and verify its truth table in Quartus using Verilog programming.

## Equipments Required:
## Hardware – PCs, Cyclone II , USB flasher
## Theory
Subtractor circuits take two binary numbers as input and subtract one binary number input from the other binary number input. Similar to adders, it gives out two outputs, difference and borrow (carry-in the case of Adder). There are two types of subtractors.

## Half Subtractor Full Subtractor
## Half Subtractor
The half-subtractor is a combinational circuit which is used to perform subtraction of two bits. It has two inputs, X (minuend) and Y (subtrahend) and two outputs D (difference) and B (borrow). To perform x - y, we have to check the relative magnitudes of x and y. If x ;;, y, we have three possibilities: 0 - 0 = 0, 1 - 0 = 1, and 1 - I = 0. The result is called the difference bit. If x < y, we have 0 - I, and it is necessary to borrow a 1 from the next higher stage. The I borrowed from the next higher stage adds 2 to the minuend bit, just as in the decimal system a borrow adds 10 to a minuend digit. With the minuend equal to 2, the difference becomes 2 - I = 1. The half-subtractor needs two outputs. One output generates the difference and will be designated by the symbol D. The second output, designated B for borrow, generates the binary signal that informs the next stage that a I has been borrowed.
![image](https://github.com/pavithraselvaraj30/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/149366880/e0532a8d-7a90-4f66-95b9-ffedc87f42ef)

Sum = X'Y+XY' = X ⊕ Y Carry=X'Y

## Full Subtractor
A full subtractor is a combinational circuit that performs subtraction involving three bits, namely minuend, subtrahend, and borrow-in . It accepts three inputs: minuend, subtrahend and a borrow bit and it produces two outputs: difference and borrow. 
![image](https://github.com/pavithraselvaraj30/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/149366880/8bdfe1ed-1bbd-45fc-ad4f-f0452b92252e)


Diff = A ⊕ B ⊕ Bin B = A'Bin + A'B + BBin

## Procedure
Use module projname(input,output) to start the Verilog programming. 
2.Assign inputs and outputs using the word input and output respectively.
3.Use defined keywords like wire,assign and required logic gates to represent the boolean expression.
4.Use each output to represent one for difference and the other for borrow. 
5.End the verilog program using keyword endmodule



Write the detailed procedure here 


## Program:
Program to design a half subtractor and full subtractor circuit and verify its truth table in quartus using Verilog programming.
Developed by: Pavithra.S 
RegisterNumber: 212223230147 

```
/*
module halfsub(a,b,difference,borrow);
input a,b;
output difference,borrow;
assign difference = (a^b);
assign borrow = (~a&b);
endmodule
module fullsub(a,b,c,difference,borrow);
input a,b,c;
output difference,borrow;
assign difference=(a^b^c);
assign borrow=(~a&(b^c)|(b&c));
endmodule
*/
```

## Output:
## Truthtable:
## Half Subtractor:
![image](https://github.com/pavithraselvaraj30/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/149366880/58680632-9235-4403-be05-97a32ecc5f39)
## Full Subtractor:
![image](https://github.com/pavithraselvaraj30/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/149366880/df3f1473-da3b-49fe-9825-41ba0738d3d5)

##  RTL realization
## Half subtractor:
![image](https://github.com/pavithraselvaraj30/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/149366880/a553066d-e387-44f8-b8d4-555822b59f46)

## Full Subtractor:
![image](https://github.com/pavithraselvaraj30/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/149366880/329d8107-d1d2-46f5-8c2c-6fda19293c91)

## Timing diagram 
## Half subtractor:
![image](https://github.com/pavithraselvaraj30/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/149366880/9358025b-f574-43a5-9ec8-786cde23a35b)

## Full subtractor:
![image](https://github.com/pavithraselvaraj30/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/149366880/c08a55e8-4797-4142-8987-e54797b5fec8)

## Result:

Thus the half subtractor and full subtractor circuits are designed and the truth tables is verified using quartus software.
