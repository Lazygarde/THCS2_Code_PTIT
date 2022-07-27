#include <stdio.h>
int main()
{
    int t;
    scanf("%d", &t);
    for (int k = 1; k <= t; k++)
    {
        int n;
        scanf("%d", &n);
        int rb = 1, re = n, cb = 1, ce = n, x = n * n, a[n + 1][n + 1];
        while (rb <= (n + 1) / 2 && cb <= (n + 1) / 2)
        {
            for (int i = cb; i <= ce; i++)
            {
                a[rb][i] = x;
                x--;
            }
            for (int j = rb + 1; j <= re; j++)
            {
                a[j][ce] = x;
                x--;
            }
            for (int i = ce - 1; i >= cb; i--)
            {
                a[re][i] = x;
                x--;
            }
            for (int j = re - 1; j >= rb + 1; j--)
            {
                a[j][cb] = x;
                x--;
            }
            rb++;
            re--;
            cb++;
            ce--;
        }
        printf("Test %d:\n", k);
        for (int i = 1; i <= n; i++)
        {
            for (int j = 1; j <= n; j++)
                printf("%d ", a[i][j]);
            printf("\n");
        }
    }
}
