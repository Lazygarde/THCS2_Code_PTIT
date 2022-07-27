#include <stdio.h>
#include <math.h>
int check(int n)
{
    int x = 0, m = n, s = 0;
    while (n != 0)
    {
        int k = n % 10;
        x = x * 10 + k;
        s += k;
        n /= 10;
    }
    if (m == x && s % 10 == 0)
        return 1;
    return 0;
}
int main()
{
    int t;
    scanf("%d", &t);
    while (t--)
    {
        int n, s = 0;
        scanf("%d", &n);
        int p1 = pow(10, n - 1), p2 = pow(10, n);
        for (int i = p1; i < p2; i++)
            if (check(i))
                s++;
        printf("%d\n", s);
    }
}
