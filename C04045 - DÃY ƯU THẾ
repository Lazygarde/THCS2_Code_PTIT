#include <stdio.h>
#include <string.h>
int check(int a[], int n)
{
    int sc = 0, sl = 0;
    for (int i = 0; i < n; i++)
    {
        if (a[i] % 2 == 0)
            sc++;
        else
            sl++;
    }
    if (n % 2 == 0 && sc > sl)
        return 1;
    if (n % 2 != 0 && sc < sl)
        return 1;
    return 0;
}
int main()
{
    int t;
    scanf("%d\n", &t);
    while (t--)
    {
        int n = 0, a[205] = {0};
        while (scanf("%d", &a[n]) != -1)
        {
            n++;
            char c = getchar();
            if (c == '\n')
                break;
        }
        if (check(a, n))
            printf("YES\n");
        else
            printf("NO\n");
    }
}
