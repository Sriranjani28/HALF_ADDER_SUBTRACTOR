# HALF_ADDER_SUBTRACTOR

Implementation-of-Half-Adder-and-Half Subtractor-circuit

**AIM:**

To design a half adder and half subtractor circuit and verify its truth table in Quartus using Verilog programming.

**Equipments Required:**

Hardware – PCs, Cyclone II , USB flasher 

Software – Quartus prime Theory Adders are digital circuits that carry out the addition of numbers.

**Half Adder**

Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

![image](https://github.com/naavaneetha/HALF_ADDER_SUBTRACTOR/assets/154305477/bd4a0b2c-cdbc-4184-ab08-81578f121e1f)

Figure -01 HALF ADDER

**Half Subtractor**

The half-subtractor is a combinational circuit which is used to perform subtraction of two bits. It has two inputs, X (minuend) and Y (subtrahend) and two outputs D (difference) and B (borrow). To perform x - y, we have to check the relative magnitudes of x and y. If x ;;, y, we have three possibilities: 0 - 0 = 0, 1 - 0 = 1, and 1 - I = 0. The result is called the difference bit. If x < y, we have 0 - I, and it is necessary to borrow a 1 from the next higher stage. The I borrowed from the next higher stage adds 2 to the minuend bit, just as in the decimal system a borrow adds 10 to a minuend digit. With the minuend equal to 2, the difference becomes 2 - I = 1. The half-subtractor needs two outputs. One output generates the difference and will be designated by the symbol D. The second output, designated B for borrow, generates the binary signal that informs the next stage that a I has been borrowed. 

Diff = A’B+AB’ =A ⊕ B
Borrow = A’B

 ![image](https://github.com/naavaneetha/HALF_ADDER_SUBTRACTOR/assets/154305477/d76b099c-513f-4e7c-843a-e2fd028a531a)

Figure -02 HALF Subtractor

**Truthtable**
<img width="297" alt="ex 3 truth table" src="https://github.com/user-attachments/assets/1a0c6b95-95ee-4241-abdc-233a041f1cbe" />

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

/* Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
module encod_data(d, x, y, z); 
    input [7:0] d; 
    output x; 
    output y; 
    output z; 
  assign#3 x=d[4]|d[5]|d[6]|d[7]; 
  assign#3 y=d[2]|d[3]|d[6]|d[7]; 
  assign#3 z=d[1]|d[3]|d[5]|d[7];
  endmodule

Developed by: Sriranjani.M
RegisterNumber:24900016
*/

**RTL Schematic**
<img width="678" alt="ex 3 rtl" src="https://github.com/user-attachments/assets/dbba946a-4b93-4477-8d36-1490ee71078e" />


**Output/TIMING Waveform**
<img width="623" alt="ex 3 timing diagram" src="https://github.com/user-attachments/assets/9ffc6027-08d0-4782-b36a-192f40095397" />


**Result:**
Hence to design a half adder and half subtractor circuit and verified its truth table in Quartus using Verilog programming.
