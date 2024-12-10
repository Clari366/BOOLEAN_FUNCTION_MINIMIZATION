
**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**

Boolean Algebra is a branch of algebra that deals with boolean values-true and false.It is fundamental to digital logic design and computer science,providing a mathamatical framework for describing logical operation and expressions.


**Logic Diagram**

![WhatsApp Image 2024-12-10 at 8 50 19 PM](https://github.com/user-attachments/assets/561758b2-2c80-454c-acd2-714f4ba88c88)


**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by:clarissa k  RegisterNumber:*/24009830
```

module funct1(a,b,c,d,f1);
input a,b,c,d;
output f1;
assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));
endmodule
```
```
module funct2(w,x,y,z,f2);
input w,x,y,z;
output f2;
assign f2=((~y & z)|( w & y )|(x & y));
endmodule
```


**Output:**

**RTL**
f1:

![Screenshot 2024-11-05 073250](https://github.com/user-attachments/assets/7205227f-7358-49ea-89dc-702646bc5f07)



f2:

![Screenshot 2024-11-05 074550](https://github.com/user-attachments/assets/b1d130ce-a97f-43a4-bda9-9c0b688422fa)

**Timing Diagram**

f1:

![WhatsApp Image 2024-12-10 at 8 40 13 PM (1)](https://github.com/user-attachments/assets/42b60673-eab7-4974-a5b7-6b1705315e44)

f2:
![Screenshot 2024-11-05 074851](https://github.com/user-attachments/assets/e3db1534-52a8-4a04-beb4-8ff49fc32124)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

