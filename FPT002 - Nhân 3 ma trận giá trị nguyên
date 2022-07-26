#include <stdio.h>
int main()
{
    int m, n, p, q;
    scanf("%d%d%d%d", &m, &n, &p, &q);
    long long a[100][100], b[100][100], c[100][100];
    int i, j, k;
    for (i = 1; i <= m; i++)
        for (j = 1; j <= n; j++)
            scanf("%lld", &a[i][j]);
    for (i = 1; i <= n; i++)
        for (j = 1; j <= p; j++)
            scanf("%lld", &b[i][j]);
    for (i = 1; i <= p; i++)
        for (j = 1; j <= q; j++)
            scanf("%lld", &c[i][j]);
    long long res1[100][100], res2[100][100];
    for (i = 1; i <= m; i++)
    {
        for (j = 1; j <= p; j++)
        {
            res1[i][j] = 0;
            for (k = 1; k <= n; k++)
                res1[i][j] += a[i][k] * b[k][j];
        }
    }
    for (i = 1; i <= m; i++)
    {
        for (j = 1; j <= q; j++)
        {
            res2[i][j] = 0;
            for (k = 1; k <= p; k++)
                res2[i][j] += res1[i][k] * c[k][j];
        }
    }
    for (i = 1; i <= m; i++)
    {
        for (j = 1; j <= q; j++)
            printf("%lld ", res2[i][j]);
        printf("\n");
    }
}
