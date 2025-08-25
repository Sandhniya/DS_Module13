# EX 1 Display operator precedence in the infix expression.
## DATE:25.08.05
## AIM:
To write a C program to find and display the priority of the operator in the given Postfix expression

## Algorithm
1.Start the program.

2.Input the infix expression 

3.Extract each character one by one from the expression.

4.Check if the symbol is an operator 

5.If it is not an operator (like numbers), skip it.


6.Use a switch-case statement to check which operator it is.

7.For each operator, return a numeric value representing its precedence.

8.Back in main(), after receiving the priority value,

9.Match the numeric value to the meaning of priority (e.g., “Lowest Priority”, “Second Highest Priority”).

1.0Display the operator and its priority meaning.

11.Repeat the steps until all operators in the expression are processed.

12.End the program. 

## Program:
```
/*
Program to find and display the priority of the operator in the given Postfix expression

#include <stdio.h>
#include<string.h>

 /* Hint:
 int priority(char x)
{
  int result;
    if(x == '&' || x == '|')
        result=1;
        
        return result;
} Hint */

int main()
{
   char ch[100]="100 200 + 2 / 5 * 7 |";
   for(int i=0;ch[i]!='\0';i++)
   {
       if(strchr("+-*/^%&|",ch[i]))
       {
           printf("%c  ----> ",ch[i]);
           switch(priority(ch[i]))
           {
               case 4:printf("Highest Priority\n");break;
               case 3: printf("Second Highest Priority\n");break;
               case 2: printf("Second Lowest Priority\n");break;
               case 1:printf("Lowest Priority\n");break;
           }
       }
   }
    
    return 0;
   
}
   
Developed by: SANDHIYA SREE B
RegisterNumber:  212223220093
*/
```

## Output:

<img width="1126" height="306" alt="image" src="https://github.com/user-attachments/assets/b671a1f1-46a1-408f-8acc-929c653391fe" />


## Result:
Thus the C program to find and display the priority of the operator in the given Postfix expression is implemented successfully
