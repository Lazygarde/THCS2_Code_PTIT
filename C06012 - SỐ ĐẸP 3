#include <stdio.h>
#include <string.h>
int check(char a[])
{
    int n = strlen(a);
    for (int i = 0; i <= (n - 1) / 2; i++)
        if (a[i] != a[n - i - 1] || a[i] == '1' || a[i] == '4' || a[i] == '6' || a[i] == '8' || a[i] == '9')
            return 0;
    return 1;
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
