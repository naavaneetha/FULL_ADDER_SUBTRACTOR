 Developed by: NAVEEN KUMAR S
 
 RegisterNumber: 24900140



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
FULL ADDER:
![full adder truth table](https://github.com/user-attachments/assets/2b582120-04d6-4010-8fe7-198c314aabc2)

FULL SUBTRACTOR:
![full subtractor truth table](https://github.com/user-attachments/assets/df53f68d-83ef-4e3f-874f-1f7385497e80)

**Procedure**

* Open Quartus2
* open new file
* create veri log file and using tools view the logic diagram
* Then click on netlist viewer and press RTL viewer to view the OUTPUT in graph format



**Program:**

FULL ADDER:

![full adder code](https://github.com/user-attachments/assets/3f3297bf-5234-4e24-b736-ab9dd0e07ae1)

FULL SUBTRACTOR:

![full subtractor code](https://github.com/user-attachments/assets/f2e058c6-e569-4c3d-a5b0-19c993f50076)

**RTL Schematic**

FULL ADDER:

![full adder gate](https://github.com/user-attachments/assets/1964b333-8274-4179-9d60-13a6072cf896)

FULL SUBTRACTOR:

![full subtractor gates](https://github.com/user-attachments/assets/06a6d8a3-8774-4948-b2bb-109fec7065dc)

**Output Timing Waveform**
FULL ADDER:

![full adder waveform](https://github.com/user-attachments/assets/e443ca20-c0f6-4c37-bceb-9f35e0e17cf8)

FULL SUBTRACTOR:

![full subtractor table](https://github.com/user-attachments/assets/f0a25356-f264-458b-a1cc-d0f52bd34239)

**Result:**

Thus the Full Adder and Full Subtractor circuits are designed and the truth tables is verified using Quartus software.



