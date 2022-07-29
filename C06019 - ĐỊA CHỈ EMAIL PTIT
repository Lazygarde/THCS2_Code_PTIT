#include <stdio.h>
#include <string.h>
int main()
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
        {
            if (s[i] >= 'A' && s[i] <= 'Z')
                s[i] += 32;
            a[n][p++] = s[i];
        }
    }
    a[n][p] = 0;
    for (int i = 0; i < n; i++)
        printf("%c", a[i][0]);
    printf("%s@ptit.edu.vn", a[n]);
}
