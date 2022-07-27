#include <stdio.h>
long long min(long long x)
{
    int n = 0, a[20];
    long long ans = 0;
    while (x > 0)
    {
        int k = x % 10;
        x /= 10;
        if (k == 6)
            a[n] = 5;
        else
            a[n] = k;
        n++;
    }
    for (int i = n - 1; i >= 0; i--)
        ans = ans * 10 + a[i];
    return ans;
}
long long max(long long x)
{
    int n = 0, a[20];
    long long ans = 0;
    while (x > 0)
    {
        int k = x % 10;
        x /= 10;
        if (k == 5)
            a[n] = 6;
        else
            a[n] = k;
        n++;
    }
    for (int i = n - 1; i >= 0; i--)
        ans = ans * 10 + a[i];
    return ans;
}
int main()
{
    int t;
    scanf("%d", &t);
    while (t--)
    {
        long long a, b;
        scanf("%lld%lld", &a, &b);
        printf("%lld %lld\n", min(a) + min(b), max(a) + max(b));
    }
}
