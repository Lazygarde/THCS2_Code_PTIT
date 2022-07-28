#include <stdio.h>
#include <string.h>
int main()
{
    int n1 = 0, p1 = 0, n2 = 0, p2 = 0;
    char s1[200], s2[200], a[100][100], b[100][100];
    gets(s1);
    gets(s2);
    int m1 = strlen(s1), m2 = strlen(s2);
    for (int i = 0; i < m1; i++)
    {
        if (s1[i] == ' ')
        {
            a[n1][p1] = 0;
            n1++;
            p1 = 0;
        }
        else
            a[n1][p1++] = s1[i];
    }
    a[n1][p1] = 0;
    for (int i = 0; i < m2; i++)
    {
        if (s2[i] == ' ')
        {
            b[n2][p2] = 0;
            n2++;
            p2 = 0;
        }
        else
            b[n2][p2++] = s2[i];
    }
    b[n2][p2] = 0;
    for (int i = 0; i <= n1; i++)
        for (int j = i + 1; j <= n1; j++)
            if (strcmp(a[i], a[j]) == 0)
                a[j][0] = 0;
    for (int i = 0; i <= n1; i++)
    {
        for (int j = i + 1; j <= n1; j++)
        {
            if (strcmp(a[i], a[j]) > 0)
            {
                char x[200];
                strcpy(x, a[i]);
                strcpy(a[i], a[j]);
                strcpy(a[j], x);
            }
        }
    }
    for (int i = 0; i <= n1; i++)
    {
        int ok = 1;
        for (int j = 0; j <= n2; j++)
        {
            if (strcmp(a[i], b[j]) == 0)
            {
                ok = 0;
                break;
            }
        }
        if (ok)
            printf("%s ", a[i]);
    }
}
