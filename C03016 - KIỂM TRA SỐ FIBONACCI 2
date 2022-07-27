#include <stdio.h>
int main()
{
    int t;
    scanf("%d", &t);
    while (t--)
    {
        long long n, a = 0, b = 1, c;
        scanf("%lld", &n);
        while (a < n)
        {
            c = a + b;
            b = a;
            a = c;
        }
        if (n == a)
            printf("YES\n");
        else
            printf("NO\n");
    }
}
