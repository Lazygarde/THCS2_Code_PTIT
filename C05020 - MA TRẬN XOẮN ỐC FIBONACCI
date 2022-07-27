#include <stdio.h>
int a[100][100];
long long b[100];
void fibo()
{
    b[0] = 0;
    b[1] = 1;
    for (int i = 2; i < 100; i++)
        b[i] = b[i - 1] + b[i - 2];
}
int main()
{
    fibo();
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
    for (int i = 1; i <= n; i++)
    {
        for (int j = 1; j <= n; j++)
            printf("%d ", a[i][j]);
        printf("\n");
    }
}
