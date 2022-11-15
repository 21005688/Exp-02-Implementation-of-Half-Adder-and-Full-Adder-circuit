# Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit

# Implementation-of-Half-Adder-and-Full-Adder-circuit
### AIM:
To design a half adder and full adder circuit and verify its truth table in Quartus using Verilog programming.

### Equipments Required:
Hardware – PCs, Cyclone II , USB flasher
Software – Quartus prime
Theory
Adders are digital circuits that carry out addition of numbers.

### Half Adder
Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

### Full Adder
Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin Carry = AB + ACin + BCin

 ![image](https://user-images.githubusercontent.com/36288975/163552156-a13e5a56-c638-4110-97d9-8896907c8d25.png)

#### Figure -01 HALF ADDER 


![image](https://user-images.githubusercontent.com/36288975/163552057-b3547877-6d07-45b4-b7e0-bcfebfad9e1d.png)

#### Figure -02 FULL ADDER 

### Procedure

1. Connect the supply (+5V) to the circuit
2. Switch ON the main switch
3. If the output is 1, then the led glows.
### 
Program:
/*
```
Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
Developed by: J.DEEPIKA
RegisterNumber: 212221230016

HALF ADDER

module Adder(a,b,sum,carry);
input a,b;
output sum,carry;
xor(sum,a,b);
and(carry,a,b);
endmodule 

FULL ADDER

module FullAdder(a,b,c,sum,carry);
input a,b,c;
output sum,carry;
assign sum = ((a^b)^c);
assign carry = ((a&b)|(b&c)|(c&a));
endmodule
```
*/
Logic symbol & Truthtable
RTL realization

### Output:

### HALF ADDER:

![HALF](https://user-images.githubusercontent.com/94747031/201806301-bb3e6d28-7be2-4b69-bbda-bb6973a6aecf.png)

### RTL:
![RLT](https://user-images.githubusercontent.com/94747031/201806367-986fbd93-517f-4ba5-9480-23b128f70c8f.png)
![INT OUT](https://user-images.githubusercontent.com/94747031/201806404-820b832b-9aef-4881-80b6-782567a3112b.png)

### TIMING DIAGRAM

![TIME](https://user-images.githubusercontent.com/94747031/201806417-2173d7e8-93f6-4dc8-b784-dfed9a189f05.png)

### FULL ADDER:

![FULL](https://user-images.githubusercontent.com/94747031/201806514-2598545e-4339-4b5c-9e83-e23b180e830a.png)

![FULL OUT](https://user-images.githubusercontent.com/94747031/201806554-dbba06c7-03f3-4e12-9e72-c08a5a90d14c.png)

## TRUTH TABLE:

![TRUTH](https://user-images.githubusercontent.com/94747031/201806630-46e26ca6-85b5-4740-a21c-6c44c5a0cc1e.png)

## TIMING DIAGRAM:
![TIMER 2](https://user-images.githubusercontent.com/94747031/201806678-7f6d44d0-bbf6-466c-8a2b-06e4340883b2.png)


### Result:
Thus, a half adder and full adder circuit is designed to verify its truth table in Quartus using Verilog programming.
