# Ex4 Evaluation of prefix expression
## DATE:24.2.2025
## AIM:
To write a C function to evaluate the given prefix expression using stack and print the output of the given prefix expression from the stack inside the function . 

## Algorithm:

1.Start the program.

2.Initialize an empty stack s and a variable top to track the top index of the stack.

3.Define a push(value) function to add an element to the stack.

4.Define a pop() function to remove and return the top element from the stack.

5.Define a function evalprefix(expression) to evaluate the prefix expression:
a. Loop through the characters of the expression from right to left.
b. For each character:
i. If the character is an operator (+, *), pop two operands from the stack, perform the operation, and push the result back onto the stack.
ii. If the character is a digit, convert it to an integer and push it onto the stack.

6.After the loop ends, the final result is at the top of the stack. Print the result.

7.End the program.



## Program:
```
#include<stdio.h>
#include<string.h>
#include<ctype.h>
int s[50];
int top=0;
void push(int ch)
{
top++;
s[top]=ch;
}
int pop()
{
int ch;
ch=s[top];
top=top-1;
return(ch);
}
void evalprefix(char p[50])
{
int a,b,c,i;
for(i=strlen(p)-1;i>=0;i--)
{
if(p[i]=='+')
{
a=pop();
b=pop();
c=a+b;
push(c);
}
else if(p[i]=='*')
{
a=pop();
b=pop();
c=a*b;
push(c);
}
else
{
push(p[i]-48);
}
}
printf("%d",pop());
}
Developed by: DHARSHINIYAA KS
RegisterNumber:  212223100004

```

## Output:

![image](https://github.com/user-attachments/assets/a0ab005f-8d30-4540-aa25-49c747051563)


## Result:
Thus, the C program to evaluate the prefix expression using stack and print the output of the given prefix expression from the stack inside the function is implemented successfully.
