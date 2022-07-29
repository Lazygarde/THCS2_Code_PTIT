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
        int l, r;
        long long s = 1;
        scanf("%d%d", &l, &r);
        for (long long i = l; i <= r; i++)
            s = lcm(s, i);
        printf("%lld\n", s);
    }
}
