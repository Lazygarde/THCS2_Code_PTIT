#include <stdio.h>
int a[2000005];
void era()
{
    for (int i = 2; i * i <= 2000000; i++)
        if (!a[i])
            for (int j = i * i; j <= 2000000; j += i)
                if (!a[j])
                    a[j] = i;
    for (int i = 2; i <= 2000000; i++)
        if (!a[i])
            a[i] = i;
}
int main()
{
    era();
    int n, x;
    long long s = 0;
    scanf("%d", &n);
    for (int i = 0; i < n; i++)
    {
        scanf("%d", &x);
        while (x != 1)
        {
            s += a[x];
            x /= a[x];
        }
    }
    printf("%lld", s);
}
