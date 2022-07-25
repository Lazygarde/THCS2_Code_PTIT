#include <stdio.h>
int main()
{
    int t;
    scanf("%d", &t);
    while (t--)
    {
        int n, s = 0;
        scanf("%d", &n);
        for (int i = 1; i * i <= n; i++)
        {
            if (n % i == 0)
            {
                if (i % 2 == 0)
                    s++;
                if (i * i != n && (n / i) % 2 == 0)
                    s++;
            }
        }
        printf("%d\n", s);
    }
}
