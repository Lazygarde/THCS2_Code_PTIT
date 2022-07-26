#include <stdio.h>
int d[100005];
void era()
{
    d[1] = 1;
    for (int i = 2; i * i <= 100000; i++)
        if (!d[i])
            for (int j = i * i; j <= 100000; j += i)
                d[j] = 1;
}
int main()
{
    era();
    int t;
    scanf("%d", &t);
    for (int k = 1; k <= t; k++)
    {
        int n;
        scanf("%d", &n);
        int a[n + 1], f[100005] = {};
        for (int i = 1; i <= n; i++)
        {
            scanf("%d", &a[i]);
            if (!d[a[i]])
                f[a[i]]++;
        }
        printf("Test %d:\n", k);
        for (int i = 1; i <= 100000; i++)
            if (f[i] != 0)
                printf("%d xuat hien %d lan\n", i, f[i]);
    }
}
