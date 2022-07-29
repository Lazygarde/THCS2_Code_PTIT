#include <stdio.h>
int main()
{
    int t;
    scanf("%d", &t);
    while (t--)
    {
        int n, p, m, x = 0;
        scanf("%d%d", &n, &p);
        for (int i = 2; i <= n; i++)
        {
            m = i;
            while (m % p == 0)
            {
                x++;
                m /= p;
            }
        }
        printf("%d\n", x);
    }
}
