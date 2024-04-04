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

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by: RegisterNumber: 212223220034*/
module ex02(A,B,C,D,F1);
input A,B,C,D;
output F1;
wire x1,x2,x3,x4,x5;
assign x1=(~A)&(~B)&(~C)&(~D);
assign x2=(A)&(~C)&(~D);
assign x3=(~B)&(C)&(~D);
assign x4=(~A)&(B)&(C)&(D);
assign x5=(B)&(~C)&(D);
assign F1=x1|x2|x3|x4|x5;
endmodule
**Truth table**
![Screenshot 2024-04-04 083113](https://github.com/hema-dharshini5/BOOLEAN_FUNCTION_MINIMIZATION/assets/147117728/3ed2397c-9c2b-49e8-bde8-0a4749c0b459)
**RTL realization**
![Screenshot 2024-04-04 083139](https://github.com/hema-dharshini5/BOOLEAN_FUNCTION_MINIMIZATION/assets/147117728/70da1d15-5f39-4399-a8cf-c1d2d602b464)
**Output:**

![Screenshot 2024-04-04 083157](https://github.com/hema-dharshini5/BOOLEAN_FUNCTION_MINIMIZATION/assets/147117728/1ed90bc9-90f5-4041-8367-fba583e7aa6e)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

