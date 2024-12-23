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

**BOOLEAN MINIMIZATION**
![Screenshot 2024-12-23 214955](https://github.com/user-attachments/assets/f0ac3ad4-60bb-44b3-a5b8-56ad7de8d2ec)
![Screenshot 2024-12-23 215047](https://github.com/user-attachments/assets/64839c1d-9fb3-4fb8-9a34-e0009e0d39a8)

**TRUTH TABLE**

![Screenshot 2024-12-23 215249](https://github.com/user-attachments/assets/a733b4de-69c7-4f53-94a6-7217d016f624)


**Program:**
i)
module funct1(a,b,c,d,f1);

input a,b,c,d;

output f1;

assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));

endmodule

ii)
module funct2(w,x,y,z,f2);

input w,x,y,z;

output f2;

assign f2=((~y & z)|( w & y )|(x & y));

endmodule

Developed by:KISHOR K R RegisterNumber:24003621

**RTL**

![Screenshot 2024-12-23 215531](https://github.com/user-attachments/assets/9e44f80a-f174-43fe-af3d-9a921b1e36ca)

**Timing Diagram**


![Screenshot 2024-12-23 215650](https://github.com/user-attachments/assets/4aaa5c4e-cc6f-48fa-8291-a89d6ab07497)


**Result:**

Thus the given logic functions are implemented using and their operations are verified
using Verilog programming.
