#include <stdio.h>
void in(int n, int k, int ok)
{
    if (ok)
        printf(" * ");
    printf("%d^%d", n, k);
}
int main()
{
    int t;
    scanf("%d", &t);
    while (t--)
    {
        int n, ok = 0;
        scanf("%d", &n);
        printf("%d = ", n);
        for (int i = 2; i * i <= n; i++)
        {
            int s = 0;
            while (n % i == 0)
            {
                s++;
                n /= i;
            }
            if (s > 0)
            {
                in(i, s, ok);
                if (!ok)
                    ok = 1;
            }
        }
        if (n > 1)
            in(n, 1, ok);
        printf("\n");
    }
}
