# Ex5 Stack Operations
## DATE:25.08.25
## AIM:
To write a C function to perform push and pop operation of the stack in the infix to postfix conversion.

## Algorithm
1. Push

If stack full → Overflow.

Else top = top + 1, insert element at stack[top].

2.Pop

If stack empty → Underflow.

Else take element from stack[top], then top = top - 1.
## Program:
```
/*
Program to find and display the priority of the operator in the given Postfix expression
#include<stdio.h>

char stack[100];
int top = -1;

void push(char x)
{
   stack[++top]=x;
}

char pop()
{
   if(top==-1)
   return -1;
   else
   return stack[top--];
}
Developed by: SANDHIYA SREE B
RegisterNumber:  212223220093
*/
```

## Output:


<img width="1153" height="357" alt="image" src="https://github.com/user-attachments/assets/95899b64-049f-4d1e-ad8b-ba421216e944" />

## Result:
Thus the C program to perform push and pop operation of the stack in the infix to postfix conversion is implemented successfully.
