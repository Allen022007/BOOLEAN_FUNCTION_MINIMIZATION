# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**

![Theory](https://github.com/user-attachments/assets/e29e09d3-ec1a-4579-b52f-4f5f922a9606)


**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

~~~
module EXP_2(a,b,c,d,w,x,y,z,f1,f2);
input a,b,c,d,w,x,y,z;
output f1,f2;
assign f1=((~b&~d)|(~a&b&d)|(a&b&~c));
assign f2=((~y&z)|(x&y)|(w&y));
endmodule
~~~

Developed by: W Allen Johnston Ozario
RegisterNumber: 24900645


**RTL realization Output:**

![EXP_2](https://github.com/user-attachments/assets/5fb60f99-1c31-4dc9-954b-c42076b74d8b)


**Timing Diagram**

![waveform](https://github.com/user-attachments/assets/c1532379-5808-4d3b-b648-04c8cb08933e)


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

