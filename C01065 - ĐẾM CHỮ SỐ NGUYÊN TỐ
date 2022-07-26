#include <stdio.h>
int main()
{
    long long n, m = 0;
    scanf("%lld", &n);
    int p = 0, a[15], f[15] = {};
    while (n)
    {
        m = m * 10 + n % 10;
        n /= 10;
    }
    n = m;
    while (n != 0)
    {
        int k = n % 10;
        n /= 10;
        if (k != 2 && k != 3 && k != 5 && k != 7)
            continue;
        if (f[k] == 0)
            a[p++] = k;
        f[k]++;
    }
    for (int i = 0; i < p; i++)
        printf("%d %d\n", a[i], f[a[i]]);
}
