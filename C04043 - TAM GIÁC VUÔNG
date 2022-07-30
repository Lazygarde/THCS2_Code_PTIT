#include <stdio.h>
#include <math.h>
int main()
{
    int t;
    scanf("%d", &t);
    while (t--)
    {
        int n, ok = 0;
        scanf("%d", &n);
        long long a[n];
        for (int i = 0; i < n; i++)
            scanf("%lld", &a[i]);
        for (int i = 0; i < n - 2; i++)
        {
            for (int j = i + 1; j < n - 1; j++)
            {
                long long k = sqrt(a[i] * a[i] + a[j] * a[j]);
                if (k == sqrt(a[i] * a[i] + a[j] * a[j]))
                {
                    for (int y = j + 1; y < n; y++)
                    {
                        if (a[y] == k)
                        {
                            ok = 1;
                            printf("YES\n");
                            break;
                        }
                    }
                }
                if (ok == 1)
                    break;
            }
            if (ok == 1)
                break;
        }
        if (ok == 0)
            printf("NO\n");
    }
}
