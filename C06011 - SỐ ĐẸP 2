#include <stdio.h>
#include <string.h>
int check(char a[])
{
    int s = 0, n = strlen(a);
    for (int i = 0; i <= (n - 1) / 2; i++)
    {
        if (a[i] != a[n - i - 1])
            return 0;
        s += a[i] - '0';
    }
    if (a[0] == '8' && s % 10 == 0)
        return 1;
    return 0;
}
int main()
{
    int t;
    scanf("%d", &t);
    while (t--)
    {
        char a[1000];
        scanf("%s", a);
        if (check(a))
            printf("YES\n");
        else
            printf("NO\n");
    }
}
