#include <stdio.h>
int main()
{
    int n, a, b;
    scanf("%d", &n);
    int su = 0, sd = 0, mxu = 0, mxd = 0, mu = 1e9, md = 1e9;
    for (int i = 1; i <= n; i++)
    {
        scanf("%d%d", &a, &b);
        su += a;
        sd += b;
        if (a < mu)
            mu = a;
        else if (a > mxu)
            mxu = a;
        if (b < md)
            md = b;
        else if (b > mxd)
            mxd = b;
    }
    if (su < sd)
    {
        sd += mu;
        printf("%d", sd);
    }
    else if (su > sd)
    {
        su += md;
        printf("%d", su);
    }
    else
    {
        su += mxd;
        sd += mxu;
        if (su < sd)
            printf("%d", su);
        else
            printf("%d", sd);
    }
}
