#include <stdio.h>
int main()
{
    int t;
    scanf("%d", &t);
    for (int k = 1; k <= t; k++)
    {
        int n, m, max = 0, mh, mc;
        scanf("%d%d", &n, &m);
        int a[n + 1][m + 1], h[n + 1], c[m + 1];
        for (int i = 1; i <= n; i++)
            h[i] = 0;
        for (int i = 1; i <= m; i++)
            c[i] = 0;
        for (int i = 1; i <= n; i++)
        {
            for (int j = 1; j <= m; j++)
            {
                scanf("%d", &a[i][j]);
                h[i] += a[i][j];
                c[j] += a[i][j];
            }
        }
        for (int i = 1; i <= n; i++)
        {
            if (max < h[i])
            {
                max = h[i];
                mh = i;
            }
        }
        max = 0;
        for (int i = 1; i <= m; i++)
        {
            if (max < c[i] - a[mh][i])
            {
                max = c[i] - a[mh][i];
                mc = i;
            }
        }
        printf("Test %d:\n", k);
        for (int i = 1; i <= n; i++)
        {
            if (i != mh)
            {
                for (int j = 1; j <= m; j++)
                    if (j != mc)
                        printf("%d ", a[i][j]);
                printf("\n");
            }
        }
    }
}
