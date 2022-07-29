#include <stdio.h>
#include <string.h>
int check(char a[], char b[])
{
    char s1[205], s2[205];
    strcpy(s1, a);
    strcpy(s2, b);
    for (int i = 0; i < strlen(s1); i++)
        if (s1[i] >= 'A' && s1[i] <= 'Z')
            s1[i] += 32;
    for (int i = 0; i < strlen(s2); i++)
        if (s2[i] >= 'A' && s2[i] <= 'Z')
            s2[i] += 32;
    if (strcmp(s1, s2))
        return 1;
    return 0;
}
int main()
{
    int t;
    scanf("%d\n", &t);
    for (int z = 1; z <= t; z++)
    {
        int n = 0, p = 0;
        char s[205], x[50], a[205][205];
        gets(s);
        gets(x);
        for (int i = 0; i < strlen(s); i++)
        {
            if (s[i] == ' ')
            {
                a[n][p] = 0;
                if (p != 0)
                    n++;
                p = 0;
            }
            else
                a[n][p++] = s[i];
        }
        a[n][p] = 0;
        printf("Test %d: ", z);
        for (int i = 0; i <= n; i++)
            if (check(a[i], x))
                printf("%s ", a[i]);
        printf("\n");
    }
}
