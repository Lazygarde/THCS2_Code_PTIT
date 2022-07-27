#include <stdio.h>
int check(int n)
{
    int x = 0, m = n;
    while (n != 0)
    {
        int k = n % 10;
        if (k == 9)
            return 0;
        x = x * 10 + k;
        n /= 10;
    }
    if (m == x)
        return 1;
    return 0;
}
int main()
{
    int n, s = 0;
    scanf("%d", &n);
    for (int i = 2; i < n; i++)
    {
        if (check(i))
        {
            s++;
            printf("%d ", i);
        }
    }
    printf("\n%d", s);
}
