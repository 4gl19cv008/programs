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
void prime (int terms)
 {
   
    int n = 30;
    int cnt = 0;
    if (n <= 1)
        printf("%d is NOT prime\n", n);
    else {
        for (int i = 1; i <= n; i++) {
            if (n % i == 0)
                cnt++;
        }
        if (cnt > 2)
            printf("%d is NOT prime\n", n);
        else
            printf("%d is prime", n);
    }
 return 0;
}
