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
module Boolean_min(A,B,C,D,W,X,Y,Z,F1,F2);
input A,B,C,D,W,X,Y,Z;
wire x1,x2,x3,x4,x5,x6,x7,x8,x9,x10;
output F1,F2;
assign x1=(~A)&(~B)&(~C)&(~D);
assign x2=(A)&(~C)&(~D);
assign x3=(~B)&(C)&(~D);
assign x4=(~A)&(B)&(C)&(D);
assign x5=(B)&(~C)&(D);
assign x6=(X)&(~Y)&(Z);
assign x7=(~X)&(~Y)&(Z);
assign x8=(~W)&(X)&(Y);
assign x9=(W)&(~X)&(Y);
assign x10=(W)&(X)&(Y);
assign F1=x1|x2|x3|x4|x5;
assign F2=x6|x7|x8|x9|x10;
endmodule
```


 Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by: Shivani M RegisterNumber: 24003648
**Truth Table:**
![Screenshot 2024-11-26 104124](https://github.com/user-attachments/assets/df0c9735-a524-4152-8128-c9af79e6611c)
![Screenshot 2024-11-26 104221](https://github.com/user-attachments/assets/6cd546d4-e0fc-462c-82a6-1e3adb6fdf0a)

**RTL realization**
![Screenshot 2024-11-26 104355](https://github.com/user-attachments/assets/d8c17821-9217-4340-ab18-5ae2f1e7fafb)

**RTL**

![Screenshot 2024-11-26 104342](https://github.com/user-attachments/assets/c46ebbf1-518b-4e25-ba1e-9facec7db899)


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

