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
```
module ex2 (a,b,c,d,w,x,y,z,f1,f2);
input a,b,c,d,w,x,y,z;
output f1,f2;
assign f1 = ~a&~b&~c&~d | a&~c&~d | ~b&c&~d | ~a&b&c&d | b&~c&d;
assign f2 = x&~y&z | ~x&~y&z | ~w&x&y | w&~x&y | w&x&y;
endmodule
```

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by: Jesu Joyal 
RegisterNumber:212225040154


**RTL realization**
<img width="766" height="422" alt="Screenshot 2026-09-04 105621" src="https://github.com/user-attachments/assets/76c6bf41-fa42-4bff-8cbd-5f40dd89804c" />

**Output:**


<img width="1917" height="1078" alt="Screenshot 2026-09-04 105600" src="https://github.com/user-attachments/assets/48e3358c-ea93-4a40-ab39-db24cdad526f" />


**Timing Diagram**
<img width="1917" height="1078" alt="Screenshot 2026-09-04 110152" src="https://github.com/user-attachments/assets/be482534-19ac-4498-b055-0d5ef64f052f" />


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

