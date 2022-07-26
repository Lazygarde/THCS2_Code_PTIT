#include <stdio.h>
char a[1000][1000];
int main()
{
    int t;
    scanf("%d", &t);
    while (t--)
    {
        int n, m;
        long long s = 0;
        scanf("%d%d", &n, &m);
        for (int i = 0; i < n; i++)
            scanf("%s", a[i]);
        int h1[1000] = {}, h2[1000] = {}, c1[1000] = {}, c2[1000] = {};
        for (int i = 0; i < n; i++)
        {
            for (int j = 0; j < m; j++)
            {
                if (a[i][j] == '1')
                {
                    h1[i]++;
                    c1[j]++;
                }
                else if (a[i][j] == '2')
                {
                    h2[i]++;
                    c2[j]++;
                }
            }
        }
        for (int i = 0; i < n; i++)
        {
            for (int j = 0; j < m; j++)
            {
                if (a[i][j] == '1')
                    s += h2[i] * c2[j];
                else if (a[i][j] == '2')
                    s += h1[i] * c1[j];
            }
        }
        printf("%lld\n", s);
    }
}
