#include <stdio.h>
long long gcd(long long a, long long b)
{
    while (a != 0)
    {
        long long x = a;
        a = b % a;
        b = x;
    }
    return b;
}
long long lcm(long long a, long long b)
{
    return a * b / gcd(a, b);
}
int main()
{
    int t;
    scanf("%d", &t);
    while (t--)
    {
        int n;
        long long s = 1;
        scanf("%d", &n);
        for (long long i = 1; i <= n; i++)
            s = lcm(s, i);
        printf("%lld\n", s);
    }
}
