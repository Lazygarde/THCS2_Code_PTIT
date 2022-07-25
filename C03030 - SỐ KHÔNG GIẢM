#include <stdio.h>
int n, a[10];
void Try(int k)
{
    if (k == n + 1)
    {
        for (int i = 1; i <= n; i++)
            printf("%d", a[i]);
        printf(" ");
        return;
    }
    for (int i = a[k - 1]; i <= 9; i++)
    {
        a[k] = i;
        Try(k + 1);
    }
}
int main()
{
    int t;
    scanf("%d", &t);
    a[0] = 1;
    while (t--)
    {
        scanf("%d", &n);
        Try(1);
        printf("\n");
    }
}
