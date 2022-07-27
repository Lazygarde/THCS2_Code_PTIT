#include <stdio.h>
#include <string.h>
int main()
{
    char a[100][100];
    int n = 0;
    while (scanf("%s", &a[n]) != -1)
    {
        int m = strlen(a[n]);
        for (int i = 0; i < m; i++)
            if (a[n][i] >= 'A' && a[n][i] <= 'Z')
                a[n][i] += 32;
        n++;
    }
    for (int i = 0; i < n; i++)
    {
        if (a[i][0] != 0)
        {
            int s = 1;
            for (int j = i + 1; j < n; j++)
            {
                if (strcmp(a[i], a[j]) == 0)
                {
                    s++;
                    a[j][0] = 0;
                }
            }
            printf("%s %d\n", a[i], s);
        }
    }
}
