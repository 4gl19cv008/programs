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
void fibonacci(int terms)
{
    int a = 0, b = 1, next;

    printf("Fibonacci Series: ");
    for (int i = 1; i <= terms; i++)
    {
        printf("%d ", a);
        next = a + b;
        a = b;
        b = next;
    }
    printf("\n");
}
