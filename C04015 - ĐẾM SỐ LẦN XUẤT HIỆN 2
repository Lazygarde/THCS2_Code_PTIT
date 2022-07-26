#include <stdio.h>
int main()
{
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
            f[a[i]]++;
        }
        printf("Test %d:\n", k);
        for (int i = 1; i <= n; i++)
        {
            if (f[a[i]] != 0)
            {
                printf("%d xuat hien %d lan\n", a[i], f[a[i]]);
                f[a[i]] = 0;
            }
        }
    }
}
