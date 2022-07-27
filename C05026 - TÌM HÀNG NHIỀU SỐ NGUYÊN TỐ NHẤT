#include <stdio.h>
int f[1005];
void era()
{
    f[0] = f[1] = 1;
    for (int i = 2; i * i <= 1000; i++)
        if (!f[i])
            for (int j = i * i; j <= 1000; j += i)
                f[j] = 1;
}
int main()
{
    era();
    int n;
    scanf("%d", &n);
    int a[n + 1][n + 1], b[n + 1], max = 0;
    for (int i = 1; i <= n; i++)
    {
        int s = 0;
        for (int j = 1; j <= n; j++)
        {
            scanf("%d", &a[i][j]);
            if (!f[a[i][j]])
                s++;
        }
        b[i] = s;
        if (max < s)
            max = s;
    }
    for (int i = 1; i <= n; i++)
    {
        if (b[i] == max)
        {
            printf("%d\n", i);
            for (int j = 1; j <= n; j++)
                if (!f[a[i][j]])
                    printf("%d ", a[i][j]);
            return 0;
        }
    }
}
