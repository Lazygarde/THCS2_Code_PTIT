#include <stdio.h>
#include <string.h>
void check(char s1[], char s2[], char s[], int n)
{
    char a[2000] = "\0";
    for (int d = 0; d <= 2 * n; d++)
    {
        if (!strcmp(a, s))
        {
            printf("%d\n", d);
            return;
        }
        int p = 0;
        for (int i = 0; i < n; i++)
        {
            a[p++] = s2[i];
            a[p++] = s1[i];
        }
        for (int i = 0; i < n; i++)
            s1[i] = a[i];
        for (int i = n; i < 2 * n; i++)
            s2[i - n] = a[i];
    }
    printf("-1\n");
}
int main()
{
    while (1)
    {
        int n;
        scanf("%d", &n);
        if (n == 0)
            return 0;
        char s1[1000], s2[1000], s[2000];
        scanf("%s%s%s", s1, s2, s);
        check(s1, s2, s, n);
    }
}
