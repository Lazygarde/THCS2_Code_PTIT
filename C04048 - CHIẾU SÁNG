#include <stdio.h>
int main()
{
    int n, m, k, x, s = 0;
    scanf("%d%d%d", &n, &m, &k);
    int a[n + 2];
    a[0] = 1;
    a[n + 1] = 1;
    for (int i = 1; i <= n; i++)
        a[i] = 0;
    while (m--)
    {
        scanf("%d", &x);
        int b = x + k, c = x - k;
        if (b > n)
            b = n;
        if (c <= 0)
            c = 1;
        for (int i = c; i <= b; i++)
            a[i] = 1;
    }
    for (int i = 1; i <= n; i++)
    {
        int p = 0;
        while (a[i] == 0)
        {
            p++;
            i++;
        }
        int b = p / (2 * k + 1);
        if (p % (2 * k + 1) == 0)
            s += b;
        else
            s += b + 1;
        if (p != 0)
            i--;
    }
    printf("%d", s);
}
