#include <stdio.h>
int main()
{
    int t;
    scanf("%d", &t);
    while (t--)
    {
        int n, s = 1;
        scanf("%d", &n);
        for (int i = 2; i * i <= n; i++)
        {
            if (n % i == 0)
            {
                s *= i;
                while (n % i == 0)
                    n /= i;
            }
        }
        if (n > 1)
            s *= n;
        printf("%d\n", s);
    }
}
