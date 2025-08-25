# Ex2 Conversion of the infix expression into postfix expression
## DATE:25.08.25
## AIM:
To write a C program to convert the infix expression into postfix form using stack by following the operator precedence and associative rule.

## Algorithm
1.Start and read the infix expression.

2.Create an empty stack (for operators) and an empty postfix string.

3.Scan the infix expression left to right:

4.If operand → add to postfix.

5.If operator → pop higher/equal precedence operators from stack to postfix, then push current operator.

6.If ( → push to stack.

7.If ) → pop from stack to postfix until ( is found.

8.After scanning, pop all remaining operators from stack to postfix.

9.Display the postfix expression.

10.End. 

## Program:
```
/*
Program to convert the infix expression into postfix expression
#include<stdio.h>
#include<ctype.h>

char stack[100];
int top = -1;

void push(char x)
{
  
   stack[++top] = x;
}

char pop()
{
   
    if(top==-1) {
        return -1;
    }
    else 
      return stack[top--]; 
}
int priority(char x)
{
    
    
  
       if(x=='(')
         return 0;
        else if(x=='&' || x=='|')
          return 4;
        else if(x=='+' || x=='-')
          return 2;
        else if(x=='*' || x=='/' || x=='%')
          return 5;
        else if(x=='^')
          return 9;
        
        return 0;
       
   }
    

char IntoPost(char *exp)
{
  
    char *e,x;
    e = exp;
    while(*e!='\0') {
        if (isalnum(*e)) {
            printf("%c ",*e);
        }
        else if(*e=='(') {
            push(*e);
        }
        else if(*e==')') {
            while((x=pop())!='(') {
                printf("%c ",x);
            }
        }
        else {
            while(priority(stack[top])>=priority(*e)) {
                printf("%c ",pop());
            }
            push(*e);
        }
        e++;
    }
    
    while(top != -1)
    {
        printf("%c ",pop());
      
    }
    return 0;

    
}


int main()
{
    char str[100] = "4*(2+5)*9" ;
    IntoPost(str);
    return 1;
}

Developed by: SANDHIYA SREE B
RegisterNumber:  212223220093
*/
```

## Output:

<img width="1160" height="235" alt="image" src="https://github.com/user-attachments/assets/59840ed2-8c23-48b4-8184-e835ee3c8d8e" />


## Result:
Thus, the C program to convert the infix expression into postfix form using stack by following the operator precedence and associative rule is implemented successfully.
