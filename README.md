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

Developed by: Mohamed Asil S  RegisterNumber:*/212223040112

TRUTHTABLE

![Screenshot 2024-04-25 161448](https://github.com/Mohamedasils/BOOLEAN_FUNCTION_MINIMIZATION/assets/144870445/2a6ae794-9fab-401d-9274-d00165da56ed)

![Screenshot 2024-04-25 183435](https://github.com/Mohamedasils/BOOLEAN_FUNCTION_MINIMIZATION/assets/144870445/49d8799a-99d9-461a-90fa-18f71fa3fdc7)


**RTL realization**

![Screenshot 2024-04-25 183516](https://github.com/Mohamedasils/BOOLEAN_FUNCTION_MINIMIZATION/assets/144870445/fbaec3e3-1516-49c1-a477-c1d033fa20b0)


**Output:**
![Screenshot 2024-04-25 183545](https://github.com/Mohamedasils/BOOLEAN_FUNCTION_MINIMIZATION/assets/144870445/f272d5e5-dc57-41fc-ab84-075f00aa4b42)


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

