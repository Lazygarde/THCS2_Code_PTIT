#include <stdio.h>
int nto(int n)
{
    if (n <= 1)
        return 0;
    for (int i = 2; i * i <= n; i++)
        if (n % i == 0)
            return 0;
    return 1;
}
int check(int n)
{
    int s = 0, k;
    while (n > 0)
    {
        k = n % 10;
        if (k != 2 && k != 3 && k != 5 && k != 7)
            return 0;
        s += k;
        n /= 10;
    }
    if (nto(s))
        return 1;
    return 0;
}
int main()
{
    int t;
    scanf("%d", &t);
    while (t--)
    {
        int a, b, s = 0;
        scanf("%d%d", &a, &b);
        for (int i = a; i <= b; i++)
            if (nto(i) && check(i))
                s++;
        printf("%d\n", s);
    }
}
