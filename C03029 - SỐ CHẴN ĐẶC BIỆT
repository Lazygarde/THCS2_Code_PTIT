#include <stdio.h>
int check(long long n)
{
    while (n != 0)
    {
        int k = n % 10;
        if (k % 2 == 1)
            return 0;
        n /= 10;
    }
    return 1;
}
int main()
{
    int t;
    scanf("%d", &t);
    while (t--)
    {
        long long n;
        scanf("%lld", &n);
        if (check(n))
            printf("YES\n");
        else
            printf("NO\n");
    }
}
