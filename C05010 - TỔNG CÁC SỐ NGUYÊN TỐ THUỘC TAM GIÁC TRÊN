#include <stdio.h>
int f[100005];
void era()
{
    f[0] = f[1] = 1;
    for (int i = 2; i * i <= 100000; i++)
        if (!f[i])
            for (int j = i * i; j <= 100000; j += i)
                f[j] = 1;
}
int main()
{
    era();
    int n, s = 0;
    scanf("%d", &n);
    int a[n + 1][n + 1];
    for (int i = 1; i <= n; i++)
        for (int j = 1; j <= n; j++)
            scanf("%d", &a[i][j]);
    for (int i = 1; i <= n; i++)
        for (int j = i; j <= n; j++)
            if (!f[a[i][j]])
                s += a[i][j];
    printf("%d", s);
}
