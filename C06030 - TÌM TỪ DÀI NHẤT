#include <stdio.h>
#include <string.h>
int main()
{
    int n = 0, max = 0;
    char x[50], a[10000][50];
    while (scanf("%s", a[n]) != -1)
    {
        int m = strlen(a[n]);
        if (max < m)
            max = m;
        n++;
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
            printf("%s %d %d\n", a[i], max, s);
        }
    }
}
