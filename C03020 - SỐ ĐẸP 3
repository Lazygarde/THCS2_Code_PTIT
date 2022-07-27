#include <stdio.h>
int check(int n)
{
    int x = 0, m = n, s = 0, ok = 0;
    while (n != 0)
    {
        int k = n % 10;
        if (k == 6)
            ok = 1;
        x = x * 10 + k;
        s += k;
        n /= 10;
    }
    if (m == x && ok && s % 10 == 8)
        return 1;
    return 0;
}
int main()
{
    int l, r, s = 0;
    scanf("%d%d", &l, &r);
    if (r < l)
    {
        int c = r;
        r = l;
        l = c;
    }
    for (int i = l; i <= r; i++)
        if (check(i))
            printf("%d ", i);
}
