#include <stdio.h>
#include <math.h>
int main()
{
    int n;
    scanf("%d", &n);
    for (int i = 1; i <= n; i++)
    {
        for (int j = 1; j <= n - i; j++)
            printf("~");
        for (int j = -i + 1; j <= i - 1; j++)
            printf("%d", 2 * (i - abs(j) - 1) + 2);
        printf("\n");
    }
}
