#include <stdio.h>
int a[1001];
void era()
{
    a[1] = 1;
    for (int i = 2; i * i <= 1000; i++)
        if (!a[i])
            for (int j = i * i; j <= 1000; j += i)
                a[j] = 1;
}
int main()
{
    era();
    int t;
    scanf("%d", &t);
    while (t--)
    {
        int n, x;
        scanf("%d", &n);
        for (int i = 0; i < n; i++)
        {
            scanf("%d", &x);
            if (!a[x])
                printf("%d ", x);
        }
        printf("\n");
    }
}
