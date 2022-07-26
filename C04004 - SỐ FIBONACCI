#include <stdio.h>
long long a[100];
long long fibo(int n)
{
    if(n<=2)
        return 1;
    if (a[n])
        return a[n];
    a[n] = fibo(n - 1) + fibo(n - 2);
    return a[n];
}
int main()
{
    int t;
    scanf("%d", &t);
    while (t--)
    {
        int n;
        scanf("%d", &n);
        printf("%lld\n", fibo(n));
    }
}
