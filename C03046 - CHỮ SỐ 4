#include <stdio.h>
#include <math.h>
int check(int n)
{
    int s = 0, m = n, x = 0;
    while (n != 0)
    {
        int k = n % 10;
        if (k == 4)
            return 0;
        x = x * 10 + k;
        s += x;
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
        int n;
        scanf("%d", &n);
        for (int i = pow(10, n - 1); i < pow(10, n); i++)
            if (check(i))
                printf("%d ", i);
        printf("\n");
    }
}
