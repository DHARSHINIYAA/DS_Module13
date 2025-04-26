# EX3 Implementation of Tower of Hanoi
## DATE:24.2.2025
## AIM:
To write a C program to implement Tower of Hanoi

## Algorithm
1.Start the program.

2.Define the function TOH(n, source, auxiliary, destination).

3.Inside the function, check if n > 0:
a. Recursively call TOH(n-1, source, destination, auxiliary) to move n-1 disks from the source rod to the auxiliary rod.
b. Print the move of the nth disk from the source rod to the destination rod.
c. Recursively call TOH(n-1, auxiliary, source, destination) to move n-1 disks from the auxiliary rod to the destination rod.

4.Initially call the function with TOH(n, 'A', 'B', 'C'), where 'A', 'B', and 'C' represent the rods.

5.End the program.

## Program:
```
#include<stdio.h>
void TOH(int n,char x,char y,char z)
{
if(n>0)
{
TOH(n-1,x,z,y);
printf("%c to %c",x,y);
printf("\n");
TOH(n-1,z,y,x);
}
}
int main()
{
int n=2;
TOH(n,'A','B','C');
}
Developed by: DHARSHINIYAA KS
RegisterNumber:  212223100004

```

## Output:

![Screenshot 2025-04-26 190145](https://github.com/user-attachments/assets/89532f5e-bed8-469b-8461-c4188e01886a)


## Result:
Thus, the C program to implement Tower of Hanoi using recursion is implemented successfully.
