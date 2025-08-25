# Ex4 Evaluation of prefix expression
## DATE:25.08.05
## AIM:
To write a C function to evaluate the given prefix expression using stack and print the output of the given prefix expression from the stack inside the function . 

## Algorithm
1.Read prefix expression.

2.Create empty stack.

3.Scan from right to left:

4.Operand → push.

5.Operator → pop two, apply, push result.

6.Final stack top = result.

7.Print result. 
  

## Program:
```
/*
Program to evaluate the given prefix expression

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
{ int a,b,c,i;
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
Developed by: SANDHIYA SREE B
RegisterNumber: 212223220093 
*/
```

## Output:

<img width="1158" height="299" alt="image" src="https://github.com/user-attachments/assets/1cb667e9-e6e0-45a5-beee-7cc7f5291d5c" />


## Result:
Thus, the C program to evaluate the prefix expression using stack and print the output of the given prefix expression from the stack inside the function is implemented successfully.
