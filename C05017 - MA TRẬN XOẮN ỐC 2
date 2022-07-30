#include <stdio.h>
int main()
{
    int t;
    scanf("%d", &t);
    while (t--)
    {
        int n, m;
        scanf("%d%d", &n, &m);
        int a[n + 1][m + 1];
        for (int i = 1; i <= n; i++)
            for (int j = 1; j <= m; j++)
                scanf("%d", &a[i][j]);
        int rb = 1, re = n, cb = 1, ce = m;
        while (rb <= (n + 1) / 2 && cb <= (m + 1) / 2)
        {
            for (int i = cb; i <= ce; i++)
                printf("%d ", a[rb][i]);
            for (int i = rb + 1; i <= re; i++)
                printf("%d ", a[i][ce]);
            if (re > rb)
                for (int i = ce - 1; i >= cb; i--)
                    printf("%d ", a[re][i]);
            if (ce > cb)
                for (int i = re - 1; i >= rb + 1; i--)
                    printf("%d ", a[i][cb]);
            rb++;
            cb++;
            re--;
            ce--;
        }
        printf("\n");
    }
}
