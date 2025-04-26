# EX 1 Display operator precedence in the infix expression.
## DATE:20.2.2025
## AIM:
To write a C program to find and display the priority of the operator in the given Postfix expression

## Algorithm
1. Start the program.
   
2.Define a function priority(op) that returns the priority level of a given operator.

3.Initialize a string containing a sequence of operators and operands.

4.Loop through each character in the string:
a. If the character is an operator, do the following:
i. Call the priority(op) function to get the priority of the operator.
ii. Print the operator along with its priority level.

5.End the program.


## Program:
```
/*
#include <stdio.h>
#include<string.h>
int priority(char x)
{
if(x == '&' || x == '|')
return 1;
if(x == '+' || x == '-')
return 2;
if(x == '*' || x == '/' || x == '%')
return 3;
if(x == '^')
return 4;
return 0;
}
int main()
{
int i,j;
char ch[100]="(A*B)^C+(D%H)/F&G";
for(i=0;i<strlen(ch);i++)
{
if(ch[i]=='+'||
ch[i]=='-'||
ch[i]=='*'||
ch[i]=='/'||
ch[i]=='%'||
ch[i]=='^'||
ch[i]=='&'||
ch[i]=='|')
{
j=priority(ch[i]);
switch(j)
{
case 1:
printf("%c ---- > ",ch[i]);
printf("Lowest Priority\n");
break;
case 2:
printf("%c ---- > ",ch[i]);
printf("Second Lowest Priority\n");
break;
case 3:
printf("%c ---- > ",ch[i]);
printf("Second Highest Priority\n");
break;
case 4:
printf("%c ---- > ",ch[i]);
printf("Highest Priority\n");
break;
}
}
}
return 0;
}
Developed by: DHARSHINIYAA KS 
RegisterNumber: 212223100004
*/
```

## Output:

![Screenshot 2025-04-26 181328](https://github.com/user-attachments/assets/e2ff52a3-5278-4a0d-ade9-f0d25a5697c7)


## Result:
Thus the C program to find and display the priority of the operator in the given Postfix expression is implemented successfully
