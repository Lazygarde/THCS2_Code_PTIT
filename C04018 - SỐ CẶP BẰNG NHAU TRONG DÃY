#include <stdio.h>
int main()
{
    int t;
    scanf("%d", &t);
    while (t--)
    {
        int n, s = 0;
        scanf("%d", &n);
        int a[n + 1];
        a[0] = 0;
        for (int i = 1; i <= n; i++)
        {
            scanf("%d", &a[i]);
            if (a[i] == a[i - 1])
                s++;
        }
        printf("%d\n", s);
    }
}
