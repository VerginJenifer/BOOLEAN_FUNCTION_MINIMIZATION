# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**

**Logic Diagram**

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

```
Developed by: D Vergin Jenifer
RegisterNumber: 212223240174
module booleanfunc (
    input A, B, C, D,
    input w, x, y, z,
    output F1, F2
);

assign F1 = (~A & ~B & ~C & ~D) |
            (A & ~C & ~D) |
            (~B & C & ~D) |
            (~A & B & C & D) |
            (B & ~C & D);

assign F2 = (x & ~y & z) |
            (~x & ~y & z) |
            (~w & x & y) |
            (w & ~x & y) |
            (w & x & y);

endmodule
```


**RTL realization**

<img width="676" height="822" alt="image" src="https://github.com/user-attachments/assets/2ff28545-9f0a-4829-81b2-9705af15349c" />


**Output:**



**Timing Diagram**

F1:

<img width="1796" height="191" alt="image" src="https://github.com/user-attachments/assets/e05253d6-0bef-4546-81ca-b8cd54d04158" />

F2:

<img width="1802" height="146" alt="image" src="https://github.com/user-attachments/assets/30c46c75-4c97-4b9c-af5d-300e3ceeaab4" />

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

