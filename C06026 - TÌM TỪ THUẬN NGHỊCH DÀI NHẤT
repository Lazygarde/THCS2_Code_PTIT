#include <stdio.h>
#include <string.h>
int check(char a[])
{
    int n = strlen(a);
    for (int i = 0; i <= (n - 1) / 2; i++)
        if (a[i] != a[n - i - 1])
            return 0;
    return 1;
}
int main()
{
    int n = 0, max = 0;
    char x[50], a[10000][50];
    while (scanf("%s", x) != -1)
    {
        if (check(x))
        {
            int m = strlen(x);
            strcpy(a[n++], x);
            if (max < m)
                max = m;
        }
    }
    for (int i = 0; i < n; i++)
    {
        if (strlen(a[i]) == max)
        {
            int s = 1;
            for (int j = i + 1; j < n; j++)
            {
                if (!strcmp(a[i], a[j]))
                {
                    a[j][0] = 0;
                    s++;
                }
            }
            printf("%s %d\n", a[i], s);
        }
    }
}
