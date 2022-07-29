#include <stdio.h>
#include <math.h>
int n, f[1000006];
long long a[1000006];
void era()
{
    f[0] = f[1] = 1;
    for (int i = 2; i * i <= 1000000; i++)
        if (!f[i])
            for (int j = i * i; j <= 1000000; j += i)
                f[j] = 1;
    for (int i = 2; i <= 1000000; i++)
        if (!f[i])
            a[n++] = i;
}
int main()
{
    era();
    int t;
    scanf("%d", &t);
    while (t--)
    {
        int s = 0;
        long long l, r;
        scanf("%lld%lld", &l, &r);
        for (int i = 0; i < n; i++)
            if ((a[i] * a[i] >= l) && (a[i] * a[i] <= r))
                s++;
        printf("%d\n", s);
    }
}
