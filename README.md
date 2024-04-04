# FULL_ADDER_SUBTRACTOR

Implementation-of-Full-Adder-and-Full-subtractor-circuit

**AIM:**

To design a Full Adder and Full Subtractor circuit and verify its truth table in Quartus using Verilog programming.

**Equipments Required:**

Hardware – PCs, Cyclone II , USB flasher

Software – Quartus prime

**Full Adder and Full Subtractor**

**Full Adder**

Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin 

Carry = AB + ACin + BCin

![image](https://github.com/naavaneetha/FULL_ADDER_SUBTRACTOR/assets/154305477/0f30ba51-5ffb-4198-845f-18e054f675e7)

**Figure -1 FULL ADDER**

**Full Subtractor**

A full subtractor is a combinational circuit that performs subtraction involving three bits, namely minuend, subtrahend, and borrow-in . It accepts three inputs: minuend, subtrahend and a borrow bit and it produces two outputs: difference and borrow.

![image](https://github.com/naavaneetha/FULL_ADDER_SUBTRACTOR/assets/154305477/02b24f51-ab51-4304-9ad6-7b81ffc1ead5)

Diff = A ⊕ B ⊕ Bin 

Borrow out = A'Bin + A'B + BBin

**Truthtable**
FULL ADDER

![image](https://github.com/naavaneetha/FULL_ADDER_SUBTRACTOR/assets/138973069/689c398c-cc8c-461a-a577-bbf4984abf93)

FULL SUBTRACTOR

![image](https://github.com/naavaneetha/FULL_ADDER_SUBTRACTOR/assets/138973069/dd710d8e-d389-4846-b738-7f1de4820dd3)



**Procedure**
```
1.Type the program in Quartus software.

2.Compile and run the program.

3.Generate the RTL schematic and save the logic diagram.

4.Create nodes for inputs and outputs to generate the timing diagram.

5.For different input combinations generate the timing diagram.
```

**Program:**

/* Program to design a half subtractor and full subtractor circuit and verify its truth table in quartus using Verilog programming. Developed by:N.NAVYA SREE RegisterNumber:212223040138
*/
```
module full_addersub(a,b,c,sum,carry,D,Bo);
input a,b,c;
output sum,carry,D,Bo;
assign sum = a^b^c;
assign carry = (a&b)|(b&c)|(a&c);
assign D = a^b^c;
assign Bo = (~a&b)|(b&c)|(~a&c);
endmodule
```


**RTL Schematic**

![image](https://github.com/naavaneetha/FULL_ADDER_SUBTRACTOR/assets/138973069/a0d1122e-dd54-4087-a08f-73cfaec20432)


**Output Timing Waveform**

![image](https://github.com/naavaneetha/FULL_ADDER_SUBTRACTOR/assets/138973069/b414ead7-892e-4d9f-b7d6-78829c7535db)


**Result:**

Thus the Full Adder and Full Subtractor circuits are designed and the truth tables is verified using Quartus software.



