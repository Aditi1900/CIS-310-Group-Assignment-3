# CIS-310-Group-Assignment-3

Design Choices: Explanation of how you integrated the PC, Instruction Memory, IRs, Instruction Decoder, Register File, and ALU.


Control Signals: Description of how the instruction is decoded and how control signals are generated.


Testing: Include screenshots the correct operation of each component and the full processor.

Program Counter test:
![image](https://github.com/user-attachments/assets/dee95c76-a23f-4bfd-af77-01bd1fc98833)
![image](https://github.com/user-attachments/assets/cde4174e-b33b-4a02-a37d-cc0dc29c504b)

Instruction Memory:

Extended Instruction Registers (IRs):
![image](https://github.com/user-attachments/assets/64d7e070-37da-406b-8041-6d31580cb002)


Register File test:
![image](https://github.com/user-attachments/assets/86143608-5cae-4c40-a33f-5a809af3ff32)

Test shows that values are correctly written.

ALU tests:
ALU Test cases:
1. Add (A + B)
Inputs:
A = 0101 (5), B = 0011 (3)
Control: S1 = 0, S0 = 0, Cin = 0

![image](https://github.com/user-attachments/assets/9fdca4e1-6792-487c-bff1-5cde1464dbb4)

Expected Output:
D = 1000 (8)

2. Add with Carry (A + B + 1)
Inputs:
A = 0110 (6), B = 0010 (2)
Control: S1 = 0, S0 = 0, Cin = 1

![image](https://github.com/user-attachments/assets/b43e8bfc-8801-4141-bc03-fc37e477aff3)



Expected Output:
D = 1001 (9)

3. Subtract (A - B)
Inputs:
A = 1010 (10), B = 0011 (3)
Control: S1 = 0, S0 = 1, Cin = 1

![image](https://github.com/user-attachments/assets/ce06d3af-17f6-4a45-a4df-16cb4329fcd9)


Expected Output:
D = 0111 (7)

4. Subtract with Borrow (A - B - 1)
Inputs:
A = 1001 (9), B = 0010 (2)
Control: S1 = 0, S0 = 1, Cin = 0

![image](https://github.com/user-attachments/assets/a5f901ff-bfc1-41b0-b12d-a6c9aa20b977)


Expected Output:
D = 0110 (6)

5. Transfer A
Inputs:
A = 1100 (12)
Control: S1 = 1, S0 = 0, Cin = 0

![image](https://github.com/user-attachments/assets/aef35d51-ab9d-40a8-a29e-2bb62d26270f)

Expected Output:
D = 1100 (12)

6. Increment A
Inputs:
A = 0111 (7)
Control: S1 = 1, S0 = 0, Cin = 1
![image](https://github.com/user-attachments/assets/97272b46-880a-4c76-b121-f3eb93514c82)

Expected Output:
D = 1000 (8)

7. Decrement A
Inputs:
A = 1001 (9)
Control: S1 = 1, S0 = 1, Cin = 0
![image](https://github.com/user-attachments/assets/91c33cba-f73c-4ff3-9443-ffb3d34bd1d1)

Expected Output:
D = 1000 (8)



