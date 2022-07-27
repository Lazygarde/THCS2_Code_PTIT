#include <stdio.h>
int main()
{
    int n, m, x, y;
    scanf("%d%d", &n, &m);
    int a[n + 1][m + 1];
    for (int i = 1; i <= n; i++)
        for (int j = 1; j <= m; j++)
            scanf("%d", &a[i][j]);
    scanf("%d%d", &x, &y);
    for (int i = 1; i <= n; i++)
    {
        int k = a[i][x];
        a[i][x] = a[i][y];
        a[i][y] = k;
    }
    for (int i = 1; i <= n; i++)
    {
        for (int j = 1; j <= m; j++)
            printf("%d ", a[i][j]);
        printf("\n");
    }
}
