# Ex5 Stack Operations
## DATE:27.2.2025
## AIM:
To write a C function to perform push and pop operation of the stack in the infix to postfix conversion.

## Algorithm
1.Initialize top as -1 and declare stack as a character array.

2.To push an element:
a. Increment top by 1.
b. Assign the character to stack[top].

3.To pop an element:
a. If top is -1, the stack is empty; return -1 or an error indicator.
b. Otherwise, retrieve stack[top], decrement top by 1, and return the retrieved character.

4.End 

## Program:
```
char stack[100];
int top = -1;
void push(char x)
{
 stack[++top] = x;
}
char pop()
{
 if(top == -1)
 return -1;
 else
 return stack[top--];
}


Developed by: DHARSHINIYAA KS
RegisterNumber:  212223100004

```

## Output:

![image](https://github.com/user-attachments/assets/5e217f08-473f-41a6-8dc7-607342540460)


## Result:
Thus the C program to perform push and pop operation of the stack in the infix to postfix conversion is implemented successfully.
