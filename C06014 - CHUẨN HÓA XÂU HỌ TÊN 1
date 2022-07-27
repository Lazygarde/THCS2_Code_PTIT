#include <stdio.h>
#include <string.h>
int main()
{
    int t;
    scanf("%d\n", &t);
    while (t--)
    {
        int n = 0, p = 0;
        char s[100], a[100][100];
        gets(s);
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
        for (int i = 0; i <= n; i++)
        {
            if (a[i][0] >= 'a' && a[i][0] <= 'z')
                a[i][0] -= 32;
            for (int j = 1; j < strlen(a[i]); j++)
                if (a[i][j] >= 'A' && a[i][j] <= 'Z')
                    a[i][j] += 32;
            printf("%s ", a[i]);
        }
        printf("\n");
    }
}
