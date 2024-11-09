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
![Screenshot 2024-11-05 151544](https://github.com/user-attachments/assets/a290ee17-2378-4ff9-a9b2-978cdcab7bb4)
![Screenshot 2024-11-05 151611](https://github.com/user-attachments/assets/17aa7e81-702d-427b-9e9f-6ee47bc14d07)


**procedure**


Type the program in Quartus software.

Compile and run the program.

Generate the RTL schematic and save the logic diagram.

Create nodes for inputs and outputs to generate the timing diagram.

For different input combinations generate the timing diagram

**Program:**

/* Program to design a half subtractor and full subtractor circuit and verify its truth table in quartus using Verilog programming. 
Developed by:RAKESH RATHNA M
RegisterNumber:24900592
*/

**RTL Schematic**
![exp4](https://github.com/user-attachments/assets/7db7f283-3cff-49b0-a74f-4e6677510b19)
![exp5](https://github.com/user-attachments/assets/847604f5-8e6b-4829-94f0-9c24fac78fd5)




**Output Timing Waveform**
![Screenshot 2024-11-09 143650](https://github.com/user-attachments/assets/b60b63c3-123c-4c74-882b-2cda6b85aa64)
![Screenshot 2024-11-09 144654](https://github.com/user-attachments/assets/2ee40d54-5381-440b-8f45-69adbcc0f841)



**Result:**

Thus the Full Adder and Full Subtractor circuits are designed and the truth tables is verified using Quartus software.



