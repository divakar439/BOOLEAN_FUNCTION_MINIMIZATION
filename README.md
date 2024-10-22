# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**
**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**
/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming.
Developed by:divakar E
RegisterNumber:212222053001
```
module Boolean_min(a,b,c,d,w,x,y,z,f1,f2);
input a,b,c,d,w,x,y,z;
output f1,f2;
wire adash,bdash,cdash,ddash,ydash,p,q,r,s,t,u;
not(adash,a);
not(bdash,b);
not(cdash,c);
not(ddash,d);
not(ydash,y);
and(p,bdash,ddash);
and(q,adash,b,d);
and(r,a,b,cdash);
or(f1,p,q,r);
and g1(s,ydash,z);
and g2(t,x,y);
and g3(u,w,z);
or g4(f2,s,t,u);
endmodule
```

**RTL realization**
![Screenshot 2024-10-20 224320](https://github.com/user-attachments/assets/d4bea5c3-0bdc-4ecb-aebd-3756e75967e3)


**Truth table**
![Screenshot 2024-10-20 224328](https://github.com/user-attachments/assets/36225508-8300-4088-9e6f-277341d526ab)


**Timing Diagram**
![Screenshot 2024-10-20 224344](https://github.com/user-attachments/assets/98586421-0fe9-4d78-8581-8078ac75a1ce)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

