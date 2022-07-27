#include <stdio.h>
int main()
{
    int t;
    scanf("%d", &t);
    for (int k = 1; k <= t; k++)
    {
        int n;
        scanf("%d", &n);
        int a[n + 1], c[n + 1], b[n + 1][n + 1];
        a[0] = 1000;
        int p1 = 0, p2 = 1, max = 0;
        for (int i = 1; i <= n; i++)
        {
            scanf("%d", &a[i]);
            if (a[i] <= a[i - 1])
            {
                c[p1] = p2;
                p2 = 1;
                p1++;
            }
            b[p1][p2++] = a[i];
            if (p2 > max)
                max = p2;
        }
        c[p1] = p2;
        printf("Test %d:\n%d\n", k, max - 1);
        for (int i = 1; i <= p1; i++)
        {
            if (c[i] == max)
            {
                for (int j = 1; j < c[i]; j++)
                    printf("%d ", b[i][j]);
                printf("\n");
            }
        }
    }
}
