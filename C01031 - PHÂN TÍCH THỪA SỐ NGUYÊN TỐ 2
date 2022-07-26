#include <stdio.h>
int main()
{
    int n, ok = 0;
    scanf("%d", &n);
    for (int i = 2; i * i <= n; i++)
    {
        while (n % i == 0)
        {
            if (ok)
                printf("x");
            printf("%d", i);
            if (!ok)
                ok = 1;
            n /= i;
        }
    }
    if (n > 1)
    {
        if (ok)
            printf("x");
        printf("%d", n);
    }
}
