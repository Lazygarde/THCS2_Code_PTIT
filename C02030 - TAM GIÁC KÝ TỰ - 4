#include <stdio.h>
int main()
{
    int n;
    scanf("%d", &n);
    for (int i = 1; i <= n; i++)
    {
        int x = 1;
        for (int j = 1; j <= i; j++)
        {
            printf("%c", '@' - 1 + x);
            x += 2;
        }
        x -= 2;
        for (int j = 1; j <= i - 1; j++)
        {
            x -= 2;
            printf("%c", '@' - 1 + x);
        }
        printf("\n");
    }
}
