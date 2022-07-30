#include <stdio.h>
int lcm(int a, int b)
{
    int x, k = a * b;
    while (a != 0)
    {
        x = a;
        a = b % a;
        b = x;
    }
    return k / b;
}
int main()
{
    int t;
    scanf("%d", &t);
    while (t--)
    {
        int n;
        scanf("%d", &n);
        int a[n + 1], b[n + 2];
        for (int i = 1; i <= n; i++)
            scanf("%d", &a[i]);
        b[1] = a[1];
        for (int i = 2; i <= n; i++)
            b[i] = lcm(a[i - 1], a[i]);
        b[n + 1] = a[n];
        for (int i = 1; i <= n + 1; i++)
            printf("%d ", b[i]);
        printf("\n");
    }
}
