# HALF_ADDER_SUBTRACTOR

Implementation-of-Half-Adder-and-Half Subtractor-circuit

**AIM:**

To design a half adder and half subtractor circuit and verify its truth table in Quartus using Verilog programming.

**Equipments Required:**

Hardware – PCs, Cyclone II , USB flasher 

Software – Quartus prime Theory Adders are digital circuits that carry out the addition of numbers.

**Half Adder**

Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

![image](https://github.com/naavaneetha/HALF_ADDER_SUBTRACTOR/assets/154305477/bd4a0b2c-cdbc-4184-ab08-81578f121e1f)

Figure -01 HALF ADDER

**Half Subtractor**

The half-subtractor is a combinational circuit which is used to perform subtraction of two bits. It has two inputs, X (minuend) and Y (subtrahend) and two outputs D (difference) and B (borrow). To perform x - y, we have to check the relative magnitudes of x and y. If x ;;, y, we have three possibilities: 0 - 0 = 0, 1 - 0 = 1, and 1 - I = 0. The result is called the difference bit. If x < y, we have 0 - I, and it is necessary to borrow a 1 from the next higher stage. The I borrowed from the next higher stage adds 2 to the minuend bit, just as in the decimal system a borrow adds 10 to a minuend digit. With the minuend equal to 2, the difference becomes 2 - I = 1. The half-subtractor needs two outputs. One output generates the difference and will be designated by the symbol D. The second output, designated B for borrow, generates the binary signal that informs the next stage that a I has been borrowed. 

Diff = A’B+AB’ =A ⊕ B
Borrow = A’B

 ![image](https://github.com/naavaneetha/HALF_ADDER_SUBTRACTOR/assets/154305477/d76b099c-513f-4e7c-843a-e2fd028a531a)

Figure -02 HALF Subtractor

**Truth table for half subtractor**

![WhatsApp Image 2024-12-21 at 09 36 47_820fb12e](https://github.com/user-attachments/assets/11227597-7641-4fe9-809f-28a80aae1b50)


**Truth table for half adder**

![WhatsApp Image 2024-12-21 at 09 37 42_45da02e5](https://github.com/user-attachments/assets/23c22551-1323-472f-9b6c-138881a1d7e5)

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**


 
 HALF ADDER
```
module bye(a,b,sum,carry);
input a,b;
output sum,carry;
assign sum=(a^b);
assign carry=(a&b);
endmodulee
```
HALF SUBTRACTOR
```
module thankyou(a,b,diff,borr);
input a,b;
output diff,borr;
assign diff=(a^b);
assign borr=(~a&b);
endmodule
```
Developed by:khamalraaj S 

RegisterNumber:24901015


**RTL Schematic**

Logic Diagram for Half Addition
![Screenshot 2024-11-05 135341](https://github.com/user-attachments/assets/e45956e4-8437-46fb-8273-1784c7d05acd)

Logic Diagram for Half Subraction
![Screenshot 2024-11-05 140100](https://github.com/user-attachments/assets/94da089a-34ed-437b-8bdd-6680d59fb375)

**Output/TIMING Waveform**

Half Adder
![Screenshot 2024-11-05 135530](https://github.com/user-attachments/assets/03163037-f615-4093-9123-e1e604d9cf7d)

Half Subtractor
![Screenshot 2024-11-05 140241](https://github.com/user-attachments/assets/429005fa-59a4-49c6-bb51-b5a3ad199383)

**Result:**
Program to design a half adder and half subtractor circuit and verify its truth table in quartus using verilog programming has been done successfully
