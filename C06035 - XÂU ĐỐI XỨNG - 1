#include <stdio.h>
#include <string.h>
int check(char a[])
{
    int s = 0, n = strlen(a);
    for (int i = 0; i <= (n - 1) / 2; i++)
        if (a[i] != a[n - i - 1])
            s++;
    if ((n % 2 == 0 && s == 1) || (n % 2 == 1 && s <= 1))
        return 1;
    return 0;
}
int main()
{
    int t;
    scanf("%d\n", &t);
    while (t--)
    {
        char a[100];
        gets(a);
        if (check(a))
            printf("YES\n");
        else
            printf("NO\n");
    }
}
