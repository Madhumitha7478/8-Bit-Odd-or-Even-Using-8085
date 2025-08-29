# 8-Bit-Odd-or-Even-Using-8085

## Aim:
To write an 8085 microprocessor program to check whether a given 8-bit number is odd or even.

## Apparatus Required:
•	Laptop with an internet connection

## Algorithm:
1.	Load the number from a specified memory location into register A.
2.	Perform an AND operation with 01H to check the least significant bit (LSB).
3.	If the result is 0, the number is even; otherwise, it is odd.
4.	Store the result in a specific memory location (odd or even flag).



## Program:

```
LDA 4200H
ANI 01H
JZ L1
MVI A, 01H
JMP L2
L1: MVI A, 02H
L2: STA 4300H
HLT
```

## Output:
ODD (input):

<img width="1837" height="599" alt="Screenshot 2025-08-29 131617" src="https://github.com/user-attachments/assets/f08e7320-7dbd-42a4-b488-300909349c73" />

ODD (output):

<img width="482" height="377" alt="Screenshot 2025-08-29 131319" src="https://github.com/user-attachments/assets/57c38c2f-f41e-4d81-8010-480fecbe7951" />

EVEN (input):

<img width="1782" height="720" alt="Screenshot 2025-08-29 131343" src="https://github.com/user-attachments/assets/8b4e8e9b-31f2-44fd-878e-222b86f90ee4" />

EVEN (output):

<img width="582" height="399" alt="Screenshot 2025-08-29 131351" src="https://github.com/user-attachments/assets/e1725c55-8d71-4b60-a57a-b66b9d103de7" />





## Result:
The 8085 microprocessor successfully checks whether a given number is odd or even and stores the result in memory.

