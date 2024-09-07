# Digital-Arithmetic-Circuit
### Index
[1. Half Adder](#HalfAdder)

[2. Full Adder](#2)

[3. Full Subtractor](#3)

[4. Multiple](#4)

[5. Compare 1 Bit](#5)

[6. Compare 4 Bit](#6)

[7. Decoder 3 To 8](#7)

[8. Multiplexer 8 To 1](#8)

[9. ALU 1 Bit](#9)

<a name="HalfAdder"></a>
# **1. HALF ADDER**

A half adder is a digital logic circuit that performs binary addition of two single-bit binary numbers. It has two inputs, A and B, and two outputs SUM and Cout. Half adder logic circuits have no memory e.g 1+0; 0+1; 0+0.

## **a. Truth Table**

![Truth Table Half Adder](https://media.geeksforgeeks.org/wp-content/cdn-uploads/gq/2015/07/ha_truth-300x235.png)

## **b. Logical Expression**

*For Sum:*

![SumHA](https://media.geeksforgeeks.org/wp-content/uploads/20211017121522/xorkmap.jpg)

SUM = A xor B

*For Cout:*

![CoutHA](https://media.geeksforgeeks.org/wp-content/uploads/20211017125041/Inkedandkmap1-200x155.jpg)

Cout = A and B

Therefore we have the following logic diagram

![HA logic cỉrcuit](https://scontent.fsgn5-3.fna.fbcdn.net/v/t1.15752-9/458491565_1306045800802605_8083061287312802539_n.png?_nc_cat=104&ccb=1-7&_nc_sid=9f807c&_nc_ohc=JRbxdziXYCoQ7kNvgFkw--G&_nc_ht=scontent.fsgn5-3.fna&oh=03_Q7cD1QEaBdBqNBJYABLrSIzT_UYOL_HxkQmLnDagvodO2vSNjQ&oe=6701D854)



Similar to HA circuit, we design the FA circuit. Full Adder is the adder that adds three inputs and produces two outputs. The first two inputs are A and B and the third input is an input is an input carry as CIn. The output Carry is designated as Cout and the normal output is designated as S which is Sum.

**Full Adder Truth Table**

![Truth Table FA](https://media.geeksforgeeks.org/wp-content/uploads/2-41.jpg)

**Shorten using a Karnaugh Map**

S = A xor B xor Cin

Cout = A and B + A and Cin + B and Cin

*Full Adder Logic Circuit:*
![FA circuit](https://scontent.fsgn5-3.fna.fbcdn.net/v/t1.15752-9/457144476_2285165731823601_1387343090934048772_n.png?_nc_cat=104&ccb=1-7&_nc_sid=9f807c&_nc_ohc=dR2cok22UPIQ7kNvgGKe3bb&_nc_ht=scontent.fsgn5-3.fna&oh=03_Q7cD1QEnBzCQaQMtrCCKY1pZ8vz49XNDAwa_e1_Bue6v2pAqaw&oe=6701DA0D)
