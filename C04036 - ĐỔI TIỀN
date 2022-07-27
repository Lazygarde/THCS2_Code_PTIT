#include <stdio.h>
int main()
{
    int t;
    scanf("%d", &t);
    while (t--)
    {
        int n, s = 0;
        scanf("%d", &n);
        int a[10] = {1, 2, 5, 10, 20, 50, 100, 200, 500, 1000};
        for (int i = 9; i >= 0; i--)
        {
            while (n >= a[i])
            {
                s++;
                n -= a[i];
            }
        }
        printf("%d\n", s);
    }
}
