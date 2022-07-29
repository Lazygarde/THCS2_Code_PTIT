#include <stdio.h>
#include <string.h>
int main()
{
    int n;
    scanf("%d", &n);
    char ansname[100], name[100];
    int max = 0, k, m, c, s = 0;
    for (int i = 0; i < n; i++)
    {
        c = 0;
        scanf("%s%d%d", name, &k, &m);
        while (m / k > 0)
        {
            int a = m / k;
            c += a;
            m = m - a * k + a * 2;
        }
        if (c > max)
        {
            strcpy(ansname, name);
            max = c;
        }
        s += c;
    }
    printf("%d\n%s", s, ansname);
}
