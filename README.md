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

![WhatsApp Image 2024-12-21 at 09 37 38_358329f6](https://github.com/user-attachments/assets/ffbc6fbf-e147-40e0-af34-1e8d0e44d6ef)

![WhatsApp Image 2024-12-21 at 09 38 33_1a5d47ec](https://github.com/user-attachments/assets/c537448a-c123-4869-81ec-873d3b1b3f11)


**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**


i)HALF ADDER

```

module ha(a,b,sum,carry);
input a,b;
output sum,carry;
assign sum= (a ^ b);
assign carry= ( a & b);
endmodule

```

ii)HALF SUBTRACTOR

```


module hs(a,b,difference,borrow);
input a,b;
output difference,borrow;
assign difference= (a ^ b);
assign borrow= ( ~a & b);
endmodule

```

/* Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.

Developed by: Maebicen Kirubakar C

RegisterNumber: 24001839

**RTL Schematic**

![image](https://github.com/user-attachments/assets/eaa57342-9d41-47bd-b29e-f4708672a8a3)

![image](https://github.com/user-attachments/assets/85551dd6-bb37-4073-9119-a258336062c5)

**Output/TIMING Waveform**

![image](https://github.com/user-attachments/assets/da69aa2b-c888-4177-abd5-78b39ac7af01)


![image](https://github.com/user-attachments/assets/4e29a9bf-32ee-4abf-9bfe-457c7412d7e6)


**Result:**

Designed a half adder and half subtractor circuit and verified its truth table in Quartus using Verilog programming.


