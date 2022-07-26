#include <stdio.h>
int main()
{
    int n;
    scanf("%d", &n);
    int a[n * 2], p = n;
    for (int i = 0; i < n; i++)
    {
        a[i] = 0;
        a[i + n] = i;
    }
    for (int i = 0; i < n; i++)
    {
        for (int j = p; j < p + n; j++)
            printf("%d ", a[j]);
        printf("\n");
        p--;
    }
}
