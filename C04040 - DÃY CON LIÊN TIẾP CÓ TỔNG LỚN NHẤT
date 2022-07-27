#include <stdio.h>
int main()
{
    int t;
    scanf("%d", &t);
    while (t--)
    {
        int n, x;
        long long s = 0, max = -1e9;
        scanf("%d", &n);
        for (int i = 0; i < n; i++)
        {
            scanf("%d", &x);
            s += x;
            if (max < s)
                max = s;
            if (s < 0)
                s = 0;
        }
        printf("%lld\n", max);
    }
}
