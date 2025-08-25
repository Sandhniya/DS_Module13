# EX3 Implementation of Tower of Hanoi
## DATE:25.08.25
## AIM:
To write a C program to implement Tower of Hanoi

## Algorithm
1.If there is only one disk, just move it directly from the source rod to the destination rod.

2.If there are more than one disk:

First, move the top n-1 disks from the source rod to the auxiliary rod, using the destination as a helper.

3.Then, move the largest disk (nth disk) from the source rod to the destination rod.

4.Finally, move the n-1 disks from the auxiliary rod to the destination rod, using the source as a helper.

5.Repeat the process until all disks are moved from the source to the destination rod.   

## Program:
```
#include<stdio.h>
void TOH(int n,char x,char y,char z)
{
  if(n>0)
  {
   TOH(n-1,x,z,y);
   printf("%c to %c\n",x,y);
   TOH(n-1,z,y,x);
  }
}
int main()
{
    int n=2;
    TOH(n,'A','B','C');
    return 0;
}

Developed by: SANDHIYA SREE B
RegisterNumber:  212223220093
*/
```

## Output:


<img width="1167" height="242" alt="image" src="https://github.com/user-attachments/assets/be17a393-8ab6-477d-ba81-5704c62e2222" />


## Result:
Thus, the C program to implement Tower of Hanoi using recursion is implemented successfully.
