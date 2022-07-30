#include <stdio.h>
int a[16][16] = {0};
void swap(int n, int m)
{
    for (int i = n; i >= 1; i--)
        for (int j = m; j >= 1; j--)
            a[i][j] = 1 - a[i][j];
}
int main()
{
    int n, s = 0;
    scanf("%d", &n);
    char x;
    for (int i = 1; i <= n; i++)
    {
        scanf("\n");
        for (int j = 1; j <= n; j++)
        {
            scanf("%c", &x);
            a[i][j] = x - '0';
        }
    }
    for (int i = n; i >= 1; i--)
    {
        for (int j = n; j >= 1; j--)
        {
            if (a[i][j] == 1)
            {
                swap(i, j);
                s++;
            }
        }
    }
    printf("%d", s);
}
