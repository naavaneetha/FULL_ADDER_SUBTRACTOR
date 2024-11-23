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
![Screenshot 2024-11-23 135820](https://github.com/user-attachments/assets/4c08cf7d-a321-41d9-864a-4697eec3a907)
![Screenshot 2024-11-23 135745](https://github.com/user-attachments/assets/b4a0ab7e-1baa-4b11-9fbf-efb0d341e020)


**Procedure**
1. Type the program in Quartus software.
 2. Compile and run the program.
 3. Generate the RTL schematic and save the logic diagram.
4. Create nodes for inputs and outputs to generate the timing diagram.
 5. For different input combinations generate the timing diagram.
Write the detailed procedure here

**Program:**
```
Full Adder

module experiment42(sum,cout,a,b,cin);
output sum;
output cout;
input a;
input b;
input cin;
wire s1,c1,c2;
xor (s1,a,b);
and(c1,a,b);
xor(sum,s1,cin);
and(c2,s1,cin);
or(cout,c2,c1);
endmodule

Full Substracter


module experiment4(df,bo,a,b,bin);
output df;
output bo;
input a;
input b;
input bin;
wire w1,w2,w3;
assign w1=a^b;
assign w2=(~a&b);
assign w3=(~w1&bin);
assign df=w1^bin;
assign bo=w2|w3;
endmodule
/* Program to design a half subtractor and full subtractor circuit and verify its truth table in quartus using Verilog programming. Developed by: RegisterNumber:
*/

**RTL Schematic**
![Screenshot 2024-11-23 134805](https://github.com/user-attachments/assets/446f9e2b-d2aa-4475-9249-fb00d5581e26)
![Screenshot 2024-11-05 114359](https://github.com/user-attachments/assets/1c7acb01-654c-4dfc-b80c-c7fe17399388)

**Output Timing Waveform**
![Screenshot 2024-11-23 134955](https://github.com/user-attachments/assets/bafc5b1e-db08-4ea4-827b-0c2ef4cea19d)
![Screenshot 2024-11-05 114652](https://github.com/user-attachments/assets/373f0641-05bc-4103-a2f5-03c18f78583f)

**Result:**

Thus the Full Adder and Full Subtractor circuits are designed and the truth tables is verified using Quartus software.



