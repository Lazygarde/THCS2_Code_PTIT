#include <stdio.h>
int ucln(int a, int b)
{
    while (a != 0)
    {
        int c = a;
        a = b % a;
        b = c;
    }
    return b;
}
int main()
{
    int t;
    scanf("%d", &t);
    while (t--)
    {
        int a, b, c, d;
        scanf("%d%d%d%d", &a, &b, &c, &d);
        if (ucln(a, b) == ucln(c, d))
            printf("YES\n");
        else
            printf("NO\n");
    }
}
