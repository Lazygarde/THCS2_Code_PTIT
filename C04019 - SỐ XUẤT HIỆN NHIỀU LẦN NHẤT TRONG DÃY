#include <stdio.h>
int main()
{
    int t;
    scanf("%d", &t);
    while (t--)
    {
        int n;
        scanf("%d", &n);
        int s = 0, a[n], f[100000] = {};
        for (int i = 0; i < n; i++)
        {
            scanf("%d", &a[i]);
            f[a[i]]++;
            if (f[a[i]] > s)
                s = f[a[i]];
        }
        for (int i = 0; i < n; i++)
        {
            if (f[a[i]] == s)
            {
                f[a[i]] = 0;
                printf("%d ", a[i]);
            }
        }
        printf("\n");
    }
}
