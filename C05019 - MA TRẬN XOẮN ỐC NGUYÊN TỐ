#include <stdio.h>
int a[100][100];
int f[1000005], b[1000005];
void era()
{
    for (int i = 2; i * i <= 1000000; i++)
        if (!f[i])
            for (int j = i * i; j <= 1000000; j += i)
                f[j] = 1;
}
int main()
{
    era();
    int t, p = 0;
    scanf("%d", &t);
    for (int i = 2; i <= 1000000; i++)
        if (!f[i])
            b[p++] = i;
    for (int z = 1; z <= t; z++)
    {
        int n;
        scanf("%d", &n);
        int rb = 1, re = n, cb = 1, ce = n, k = 0;
        while (rb <= (n + 1) / 2 && cb <= (n + 1) / 2)
        {
            for (int i = cb; i <= ce; i++)
            {
                a[rb][i] = b[k];
                k++;
            }
            for (int j = rb + 1; j <= re; j++)
            {
                a[j][ce] = b[k];
                k++;
            }
            for (int i = ce - 1; i >= cb; i--)
            {
                a[re][i] = b[k];
                k++;
            }
            for (int j = re - 1; j >= rb + 1; j--)
            {
                a[j][cb] = b[k];
                k++;
            }
            rb++;
            re--;
            cb++;
            ce--;
        }
        printf("Test %d:\n", z);
        for (int i = 1; i <= n; i++)
        {
            for (int j = 1; j <= n; j++)
                printf("%d ", a[i][j]);
            printf("\n");
        }
    }
}
