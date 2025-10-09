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

<img width="585" height="663" alt="image" src="https://github.com/user-attachments/assets/4480b929-ac7e-46b4-a0d6-f4fac7f721fe" />

FULL SUBTRACTOR:

<img width="768" height="705" alt="image" src="https://github.com/user-attachments/assets/9e93e494-aea5-499b-8254-3ad509b1b512" />



**Procedure**

Full Adder:

1.Open Quartus II and create a new project.

2.Use schematic design entry to draw the full adder circuit.

3.The circuit consists of XOR, AND, and OR gates.

4.Compile the design, verify its functionality through simulation.

5.Implement the design on the target device and program it.

Full Subtractor:

1.Follow the same steps as for the full adder.

2.Draw the full subtractor circuit using schematic design.

3.The circuit includes XOR, AND, OR gates to perform subtraction.

4.Compile, simulate, implement, and program the design similarly to the full adder.

**Program:**

/* Program to design a half subtractor and full subtractor circuit and verify its truth table in quartus using Verilog programming. Developed by:NM MUTHUKUMARAN RegisterNumber:25009369
*/
Full Adder:

<img width="672" height="170" alt="Screenshot 2025-10-09 201711" src="https://github.com/user-attachments/assets/a0e7733a-c324-4b2f-b619-0cbc92e21ca4" />

Full Subtractor:

<img width="594" height="196" alt="image" src="https://github.com/user-attachments/assets/2f6fae8c-efd8-4e33-8bdd-23a86ce86c1a" />



**RTL Schematic**

Full Adder:

<img width="1920" height="918" alt="Screenshot 2025-10-08 115616" src="https://github.com/user-attachments/assets/13684b97-5180-4277-a3d3-a3ab049ebd06" />

Full Subtractor:


<img width="1747" height="506" alt="image" src="https://github.com/user-attachments/assets/e1d571a9-d20c-493d-906b-37e3a820b031" />







**Output Timing Waveform**

**Result:**

Full Adder:

<img width="1678" height="224" alt="Screenshot 2025-10-09 203801" src="https://github.com/user-attachments/assets/dae9d90d-bd34-46bb-a283-50731d02058f" />









Full Subtractor:

<img width="1873" height="265" alt="image" src="https://github.com/user-attachments/assets/85a69ee3-483b-4b9b-8339-29cc2b4be1aa" />


Thus the Full Adder and Full Subtractor circuits are designed and the truth tables is verified using Quartus software.



