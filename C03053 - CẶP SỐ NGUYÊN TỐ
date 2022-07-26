#include <stdio.h>
int a[10005];
void era()
{
    a[1] = 1;
    for (int i = 2; i * i <= 10000; i++)
        if (!a[i])
            for (int j = i * i; j <= 10000; j += i)
                a[j] = 1;
}
int main()
{
    era();
    int t;
    scanf("%d", &t);
    while (t--)
    {
        int n;
        scanf("%d", &n);
        for (int i = 2; i <= n / 2; i++)
            if (!a[i] && !a[n - i])
                printf("%d %d ", i, n - i);
        printf("\n");
    }
}
