#include <stdio.h>
int check(long long n)
{
    long long s = 0, m = n, x = 0;
    while (n != 0)
    {
        int k = n % 10;
        if (k % 2 == 0)
            return 0;
        x = x * 10 + k;
        s += k;
        n /= 10;
    }
    if (x == m && s % 2 == 1)
        return 1;
    return 0;
}
int main()
{
    int t;
    scanf("%d", &t);
    while (t--)
    {
        long long n;
        scanf("%lld", &n);
        if (check(n))
            printf("YES\n");
        else
            printf("NO\n");
    }
}
