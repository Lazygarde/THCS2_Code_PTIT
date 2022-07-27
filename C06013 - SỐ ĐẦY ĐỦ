#include <stdio.h>
#include <string.h>
char a[11] = "0123456789";
void check(char s[])
{
    int d[1000] = {}, n = strlen(s), x = 0;
    for (int i = 0; i < n; i++)
    {
        if (s[0] == '0')
        {
            printf("INVALID\n");
            return;
        }
        if (s[i] < '0' || s[i] > '9')
        {
            printf("INVALID\n");
            return;
        }
        for (int j = 0; j < 10; j++)
            if (s[i] == a[j])
                d[j]++;
    }
    for (int i = 0; i < 10; i++)
        if (d[i] != 0)
            x++;
    if (x == 0)
        printf("INVALID\n");
    else if (x == 10)
        printf("YES\n");
    else
        printf("NO\n");
}
int main()
{
    int t;
    scanf("%d", &t);
    while (t--)
    {
        char a[1005];
        scanf("%s", a);
        check(a);
    }
}
