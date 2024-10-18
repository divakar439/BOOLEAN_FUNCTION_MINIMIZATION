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

Developed by: VIJEY K S
RegisterNumber: 212223040239

```
F1
module exp02(a,b,c,d,f1);
input a,b,c,d;
output f1;
assign f1=((~b & ~d) | (a & b & ~c) | (~a & b & d));
endmodule

F2
module project22(w,x,y,z,f2);
input w,x,y,z;
output f2;
assign f2= ((~y&z)|(w&y)|(x&y));
endmodule
```

**TRUTH TABLE**
![image](https://github.com/user-attachments/assets/22370d1b-17b9-4c79-b5ad-9c9c1422cef6)

![image](https://github.com/user-attachments/assets/01a37c85-5a5d-43cb-a5dd-f9bbe50557e7)



**RTL realization**

**F1**
![new f1](https://github.com/user-attachments/assets/1146e2a2-1578-409e-b809-a3a199a9c940)




**F2**
![new f2](https://github.com/user-attachments/assets/21352699-f9ba-49c2-8dce-9c998af97902)




**Output:**

**F1**
![new f1o](https://github.com/user-attachments/assets/64961e2f-0873-424a-9f56-0bc82eee99c6)




**F2**
![new f2o](https://github.com/user-attachments/assets/6c13bd79-880d-45e6-8686-14a95fcc687f)




**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

