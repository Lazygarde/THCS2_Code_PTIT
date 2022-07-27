#include <stdio.h>
#include <string.h>
void Do(char a[], int f[])
{
    int i = 0, n = strlen(a);
    while (i < n)
    {
        int d = 0, s = 0;
        if (a[i] < '0' || a[i] > '9')
        {
            i++;
            continue;
        }
        while (i < n && a[i] >= '0' && a[i] <= '9')
        {
            d = d * 10 + a[i] - '0';
            i++;
        }
        while (a[i] < '0' || a[i] > '9')
            i++;
        while (i < n && a[i] >= '0' && a[i] <= '9')
        {
            s = s * 10 + a[i] - '0';
            i++;
        }
        f[s] += d;
    }
}
int main()
{
    int t;
    scanf("%d\n", &t);
    while (t--)
    {
        int f[10005] = {}, ok = 0;
        char a[100000], b[100000];
        gets(a);
        gets(b);
        Do(a, f);
        Do(b, f);
        for (int i = 10000; i >= 0; i--)
        {
            if (f[i])
            {
                if (ok)
                    printf(" + ");
                printf("%d*x^%d", f[i], i);
                if (!ok)
                    ok = 1;
            }
        }
        printf("\n");
    }
}
