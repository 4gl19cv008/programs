#include<stdio.h>
#include<math.h>

int main()
{
int terms;
printf("enter the number of terms:\n");
scanf("%d",&terms);

printf("the terms is %d\n",fibonacci(terms));
printf("the prime number is is %d\n",prime(terms));
return 0;
}
