#include <stdio.h>
int check(long long n)
{
    int sc = 0, sl = 0;
    if (n % 2 == 1)
        return 0;
    while (n != 0)
    {
        if ((n % 10) % 2 == 0)
            sc++;
        else
            sl++;
        n /= 10;
    }
    if (sc > sl)
        return 1;
    return 0;
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
