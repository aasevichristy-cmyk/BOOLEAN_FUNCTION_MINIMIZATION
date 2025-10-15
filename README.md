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


module funct1(a,b,c,d,f1);
input a,b,c,d;
output f1;
assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));
endmodule


module funct2(w,x,y,z,f2);
input w,x,y,z;
output f2;
assign f2=((~y & z)|( w & y )|(x & y));
endmodule



**RTL realization**

**Output:**
<img width="257" height="216" alt="image" src="https://github.com/user-attachments/assets/0a2c897f-af3c-41c0-9090-e9bdaa4411fa" />
<img width="365" height="178" alt="image" src="https://github.com/user-attachments/assets/f47f3c2d-eac2-479e-929a-fc9ac14fe118" />


**RTL**

**Timing Diagram**
<img width="1088" height="259" alt="image" src="https://github.com/user-attachments/assets/065d1348-6b32-4e56-9fac-66279ac4b1c1" />
<img width="1043" height="255" alt="image" src="https://github.com/user-attachments/assets/d63fd90a-1a48-46b3-8ba5-bbbe7ab22e19" />

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

