# FULL_ADDER_SUBTRACTOR

Implementation-of-Full-Adder-and-Full-subtractor-circuit

*AIM:*

To design a Full Adder and Full Subtractor circuit and verify its truth table in Quartus using Verilog programming.

*Equipments Required:*

Hardware – PCs, Cyclone II , USB flasher

Software – Quartus prime

*Full Adder and Full Subtractor*

*Full Adder*

Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin 

Carry = AB + ACin + BCin

![image](https://github.com/naavaneetha/FULL_ADDER_SUBTRACTOR/assets/154305477/0f30ba51-5ffb-4198-845f-18e054f675e7)

*Figure -1 FULL ADDER*

*Full Subtractor*

A full subtractor is a combinational circuit that performs subtraction involving three bits, namely minuend, subtrahend, and borrow-in . It accepts three inputs: minuend, subtrahend and a borrow bit and it produces two outputs: difference and borrow.

![image](https://github.com/naavaneetha/FULL_ADDER_SUBTRACTOR/assets/154305477/02b24f51-ab51-4304-9ad6-7b81ffc1ead5)

Diff = A ⊕ B ⊕ Bin 

Borrow out = A'Bin + A'B + BBin

*Truthtable*

*Procedure*
1.Type the program in Quartus software.
2.Compile and run the program.
3.Generate the RTL schematic and save the logic diagram.
4.Create nodes for inputs and outputs to generate the timing diagram.
5.For different input combinations generate the timing diagram.
*Program:*

/* Program to design a half subtractor and full subtractor circuit and verify its truth table in quartus using Verilog programming. 


Developed by: VISMAYA.S

RegisterNumber:212221230125
*/
## Full Adder
```
module fulladder(a,b,cin,sum,carry);
input a,b,cin;
output sum,carry;
wire w1,w2,w3,w4;       
xor(w1,a,b);
xor(sum,w1,cin);        

and(w2,a,b);
and(w3,b,cin);
and(w4,cin,a);

or(carry,w2,w3,w4);
endmodule
```
## Full Subtractor
```
module fullsub(a,b,Bin,BO,DIFF);
input a,b,Bin;
output BO,DIFF;
assign DIFF = a ^ b ^ Bin;
  assign BO = (a & b) | ((a ^ b) & Bin);
endmodule
```
*RTL Schematic*
![Screenshot 2024-03-22 143255](https://github.com/Yogesh-Yogi-1/FULL_ADDER_SUBTRACTOR/assets/148514598/939151e8-c37b-49aa-8f44-513492ba509e)
![Screenshot 2024-03-22 143433](https://github.com/Yogesh-Yogi-1/FULL_ADDER_SUBTRACTOR/assets/148514598/aa118976-fe63-40e9-a31c-cec66367d805)
*Output Timing Waveform*
![Screenshot 2024-03-18 090939](https://github.com/Yogesh-Yogi-1/FULL_ADDER_SUBTRACTOR/assets/148514598/fe08e008-070e-4e8b-bee9-f26ade621c0e)
![Screenshot 2024-03-18 092119](https://github.com/Yogesh-Yogi-1/FULL_ADDER_SUBTRACTOR/assets/148514598/c37c43ae-514e-4fda-82d9-22ed613851e0)
*Result:*

Thus the Full Adder and Full Subtractor circuits are designed and the truth tables is verified using Quartus software.
