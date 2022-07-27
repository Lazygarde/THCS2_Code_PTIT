#include <stdio.h>
int main()
{
    int t;
    scanf("%d", &t);
    while (t--)
    {
        long long n, ans;
        scanf("%lld", &n);
        for (long long i = 2; i * i <= n; i++)
        {
            if (n % i == 0)
            {
                ans = i;
                while (n % i == 0)
                    n /= i;
            }
        }
        if (n > 1)
            ans = n;
        printf("%lld\n", ans);
    }
}
