#include <stdio.h>
int main()
{
    int n, a, b;
    scanf("%d", &n);
    int minr = 1e9, minc = 1e9;
    for (int i = 0; i < n; i++)
    {
        scanf("%d%d", &a, &b);
        if (a < minr)
            minr = a;
        if (b < minc)
            minc = b;
    }
    printf("%lld", (long long)minc * minr);
}
