# Digital-Arithmetic-Circuit
### Index
[1. Half Adder](#HalfAdder)

[2. Full Adder](#FullAdder)

[3. Full Subtractor](#FullSubtractor)

[4. Multiple](#Multiple)

[5. Compare 1 Bit](#Compare1)

[6. Compare 4 Bit](#Compare4)

[7. Decoder 3 To 8](#Decoder)

[8. Multiplexer 8 To 1](#Multiplexer)

[9. ALU 1 Bit](#ALU)

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

<a name="FullAdder"></a>
# **2. FULL ADDER**

Similar to HA circuit, we design the FA circuit. Full Adder is the adder that adds three inputs and produces two outputs. The first two inputs are A and B and the third input is an input is an input carry as CIn. The output Carry is designated as Cout and the normal output is designated as S which is Sum.

## **a. Full Adder Truth Table**

![Truth Table FA](https://media.geeksforgeeks.org/wp-content/uploads/2-41.jpg)

## **b. Shorten using a Karnaugh Map**

S = A xor B xor Cin

Cout = A and B + A and Cin + B and Cin

*Full Adder Logic Circuit:*
![FA circuit](https://scontent.fsgn5-3.fna.fbcdn.net/v/t1.15752-9/457144476_2285165731823601_1387343090934048772_n.png?_nc_cat=104&ccb=1-7&_nc_sid=9f807c&_nc_ohc=dR2cok22UPIQ7kNvgGKe3bb&_nc_ht=scontent.fsgn5-3.fna&oh=03_Q7cD1QEnBzCQaQMtrCCKY1pZ8vz49XNDAwa_e1_Bue6v2pAqaw&oe=6701DA0D)

<a name="FullSubtractor"></a>
# **3. FULL SUBTRACTOR**

The full substractor is used to substract three 1-bit numbers A, B and C, which are minuend, subtrahend and borrow. The full substractor has three input states and two output states.

## **a. Full Subtractor Truth Table**

![Truth Table FS](https://javatpoint-images.s3.eu-north-1.amazonaws.com/tutorial/digital-electronics/images/full-subtractor2.png)

## **b. The SOP form can be obtained with the help of K-map as:**

Diff = xy'z' + x'y'z + xyz + x'yz'

![b1-FS-Kmap](https://javatpoint-images.s3.eu-north-1.amazonaws.com/tutorial/digital-electronics/images/full-subtractor3.png)

Borrow = x'z + x'y + yz

![b2-FS-Kmap](https://javatpoint-images.s3.eu-north-1.amazonaws.com/tutorial/digital-electronics/images/full-subtractor4.png)

*Full Subtractor Logic Circuit:*
![FS circuit](https://scontent-hkg1-2.xx.fbcdn.net/v/t1.15752-9/457804709_1463741020972293_4370423759960450823_n.png?_nc_cat=104&ccb=1-7&_nc_sid=9f807c&_nc_ohc=AWt0KGJ-GQIQ7kNvgGSoOU5&_nc_ht=scontent-hkg1-2.xx&oh=03_Q7cD1QF9nrF1-YmDzkgvSzFDt7aVhrvG1-sDZzlmYu-LDf0maw&oe=67039691)

<a name="Multiple"></a>
# **4. MULTIPLE**

We have 2 3-bit numbers A and B multiplied together; when written in detail, we will have the following expression:
                    
![Nhan3bit](https://scontent.fsgn5-5.fna.fbcdn.net/v/t1.15752-9/457045366_511072454852020_4928722400135118881_n.png?_nc_cat=100&ccb=1-7&_nc_sid=9f807c&_nc_ohc=_f_jr6IQaUoQ7kNvgGQ9Mi1&_nc_ht=scontent.fsgn5-5.fna&_nc_gid=A61akp7U-4AHP7jeYer-R9X&oh=03_Q7cD1QE-WV51LRWnrfRHpY3-UBeh3D3FZkkfDNm7lWqoqqVi6w&oe=67046A85)                

* Thus, the core circuit is essentially made up of AND gates and HA, HA.

*Multiple Circuit*

![3bitx3bit](https://scontent.fsgn5-14.fna.fbcdn.net/v/t1.15752-9/456195483_1467870113920365_6514698370964321352_n.png?_nc_cat=101&ccb=1-7&_nc_sid=9f807c&_nc_ohc=TTOTrfScQk4Q7kNvgE8fxf_&_nc_ht=scontent.fsgn5-14.fna&oh=03_Q7cD1QFAM2VyxSloXtCh0RzpNqgxoqDDeU7EXGqAnp-XkTKvcg&oe=67047E57)
