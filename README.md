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

<a name="Compare1"></a>
# **5. COMPARE 1 BIT**

For any number, to compare whether it is equal or not, we will compare each digit of that number. If each digit of that number is equal, it means that the two numbers have equal value. To compare greater than or less than, we will consider each digit in order from the digit with the largest value to the smallest.

*Compare 1 bit Circuit*
![compare1](https://scontent.fsgn5-3.fna.fbcdn.net/v/t1.15752-9/458196172_559690066388888_5164151413470968349_n.png?_nc_cat=104&ccb=1-7&_nc_sid=9f807c&_nc_ohc=da_-c_XS_SQQ7kNvgGgie-7&_nc_ht=scontent.fsgn5-3.fna&_nc_gid=ANoXD5dcPcNDEEmnLiHGs8T&oh=03_Q7cD1QFPH36a6_E-I4Jn-W2u4PfYCMYgh44vPn6XYQtzA0xB2g&oe=6705F4EE)

<a name="Compare4"></a>
# **6. COMPARE 4 BIT**

we can now combine several of the above diagrams to create a 4-bit magnitude comparator as follows:

![compare4](https://scontent.fsgn5-10.fna.fbcdn.net/v/t1.15752-9/458979673_1491145984904738_5871116225442271876_n.png?_nc_cat=110&ccb=1-7&_nc_sid=9f807c&_nc_ohc=9nXPG4qUUPoQ7kNvgHDjJ_W&_nc_ht=scontent.fsgn5-10.fna&oh=03_Q7cD1QHviwuMeogrRDI1-vKf5eAYxMLotO5LvpbFPq9NCCIcxA&oe=67060D40)

<a name="Decoder"></a>
# **7. DECODER 3 TO 8**

![decoder3to8](https://scontent.fsgn5-15.fna.fbcdn.net/v/t1.15752-9/457692844_867126752050703_9208880706017987484_n.png?_nc_cat=111&ccb=1-7&_nc_sid=9f807c&_nc_ohc=8Ct75TpIFXwQ7kNvgETFwV6&_nc_ht=scontent.fsgn5-15.fna&_nc_gid=AllyDnaM-imU6YJpmS1iHVf&oh=03_Q7cD1QHvlTZnruRUtY-YGV1D_cpNHR8HxOrsrUsrj13oDWT59Q&oe=6705FF53)

<a name="Multiplexer"></a>
# **8. MULTIPLEXER 8 TO 1**

![multiplexer](https://scontent.fsgn5-14.fna.fbcdn.net/v/t1.15752-9/458296681_8553664454643727_8452078112003587354_n.png?_nc_cat=101&ccb=1-7&_nc_sid=9f807c&_nc_ohc=sdzihsK728MQ7kNvgFQAY75&_nc_ht=scontent.fsgn5-14.fna&_nc_gid=Az-HkYOTNo8iqmHgADR-cD5&oh=03_Q7cD1QENrNSnXYwuqKBKhTU0vCVTRzP0WS-mQuDdu27AikfkFg&oe=6705F488)

<a name="ALU"></a>
# **9. ALU**

So with the above building blocks, lets construct a simple ALU that performs a arithmetic operation (1 bit addition)and does 3 logical operations namely AND, NOR and XOR as shown below. The multiplexer selects only one operation at a time. The operation selected depends on the selection lines of the multiplexer as shown in the truth table.

![alu1](https://exploreembedded.com/wiki/images/e/e9/1bitALU.jpg)

*ALU Circuit*

![alu2](https://scontent.fsgn5-12.fna.fbcdn.net/v/t1.15752-9/457785909_1241925493472196_806310001883413232_n.png?_nc_cat=103&ccb=1-7&_nc_sid=9f807c&_nc_ohc=3n8_uzVbWAEQ7kNvgGK50ji&_nc_ht=scontent.fsgn5-12.fna&_nc_gid=ALcxF1bB2btNUPllEy76szo&oh=03_Q7cD1QF1gk2zctlPa_E50NmxWEgpyLokSy2eyNypmq-2gZc7QQ&oe=6706121B)

*ALU Truth Table*
![alu3](https://scontent.fsgn5-15.fna.fbcdn.net/v/t1.15752-9/457815829_824542243190949_9182000988480758966_n.png?_nc_cat=111&ccb=1-7&_nc_sid=9f807c&_nc_ohc=TvrIu6YWfVcQ7kNvgFMdY5g&_nc_ht=scontent.fsgn5-15.fna&_nc_gid=AUJc6GcWxwO87UPPTS4jkcY&oh=03_Q7cD1QEOiz9fGgfnp8tlsNAgxmtCuvVru8H8dKwjqcqvJSSvUQ&oe=67060CCC)
