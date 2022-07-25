#include <stdio.h>
int f[1000005];
void era()
{
    f[1] = 1;
    for (int i = 2; i * i <= 1000000; i++)
        if (!f[i])
            for (int j = i * i; j <= 1000000; j += i)
                f[j] = 1;
}
int csonto(int n)
{
    while (n != 0)
    {
        int k = n % 10;
        if (k != 2 && k != 3 && k != 5 && k != 7)
            return 0;
        n /= 10;
    }
    return 1;
}
int main()
{
    era();
    int t;
    scanf("%d", &t);
    while (t--)
    {
        int a, b, s = 0;
        scanf("%d%d", &a, &b);
        for (int i = a; i <= b; i++)
            if (!f[i] && csonto(i))
                s++;
        printf("%d\n", s);
    }
}
