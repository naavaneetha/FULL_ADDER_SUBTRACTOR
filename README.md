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
Full adder:
![Screenshot 2024-12-02 193304](https://github.com/user-attachments/assets/51af2af3-3060-443c-931a-2b7b39867394)

Full subtractor:
![Screenshot 2024-12-02 193317](https://github.com/user-attachments/assets/b5ac8882-c842-4bba-84a4-4feda289c55e)

**Procedure**
```
Full Adder: 
-->Inputs: Three inputs: A, B (the two bits to be added), and Cin (the carry-in bit from a
 previous addition). 
 -->Outputs: Two outputs: Sum (the resulting sum) and Cout (the carry-out bit).
 Logic: Sum = A ^ B ^ Cin (XOR operation). Cout = (A & B) | (A & Cin) | (B & Cin) (carry occurs if at
 least two inputs are 1).
 Full Subtractor: 
 -->Inputs: Three inputs: A, B (the two bits, where A - B is calculated), and Bin (the
 borrow-in from a previous subtraction).
 -->Outputs: Two outputs: Diff (the resulting difference) and
 Bout (the borrow out bit). Logic: Diff = A ^ B ^ Bin (XOR operation). Bout = (~A & B) | ((~A | B) &
 Bin) (borrow occurs if A is less than B or needs a borrow).
 -Both circuits follow simple XOR logic for
 the primary result and AND-OR logic to determine carry or borrow conditions.
```

**Program:**

 Developed by: Rhudhra phriyamvadha KS
 RegisterNumber: 24900189
 ```
Full adder:

module fulladder(sum, cout, a, b, cin);
    output sum;
    output cout;
    input a;
    input b;
    input cin;

	 wire w1,w2,w3;
	 assign w1=a^b;
	 assign w2=a&b;
	 assign w3=w1&cin;
	 assign sum=w1^cin;
	 assign cout=w2|w3;
endmodule
```
```
Full subtractor:

module fullsub(a,b,bin,dif,bor);
 input a,b,bin;
 output dif,bor;
 assign difference=a^b^bin; 
assign borrow=~(a^b)&bin|(~a)&b;
endmodule
```
**RTL Schematic**
Full adder:
![fulladder](https://github.com/user-attachments/assets/d4d40539-a59d-43db-84d9-b35b960668f7)

Full subtractor:
![Screenshot 2024-11-28 131531](https://github.com/user-attachments/assets/47ba4dca-d043-41b9-9a2f-1659fb456ed5)

**Output Timing Waveform**
Full adder:
![waveform fulladder](https://github.com/user-attachments/assets/ae481ee6-9a65-49e6-a660-5e66ba4cf61d)


Full subtractor:
![Screenshot 2024-12-02 193104](https://github.com/user-attachments/assets/6d155d3d-96cb-4572-bd42-79b52df77d99)

**Result:**

Thus the Full Adder and Full Subtractor circuits are designed and the truth tables is verified using Quartus software.



