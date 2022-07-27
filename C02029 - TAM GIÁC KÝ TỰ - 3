#include <stdio.h>
int main()
{
    int n;
    scanf("%d", &n);
    for (int i = 1; i <= n; i++)
    {
        int x = i;
        for (int j = 1; j <= i; j++)
        {
            printf("%c ", 'A' + j + x - 2);
            x += n - j - 1;
        }
        printf("\n");
    }
}
