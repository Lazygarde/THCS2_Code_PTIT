#include <stdio.h>
int main()
{
    int n;
    scanf("%d", &n);
    int a[n];
    for (int i = 0; i < n; i++)
    {
        scanf("%d", &a[i]);
        for (int j = 0; j <= i; j++)
        {
            for (int k = i; k > j; k--)
            {
                if (a[k] < a[k - 1])
                {
                    int x = a[k];
                    a[k] = a[k - 1];
                    a[k - 1] = x;
                }
            }
        }
        printf("Buoc %d: ", i);
        for (int j = 0; j <= i; j++)
            printf("%d ", a[j]);
        if (i < n - 1)
            printf("\n");
    }
}
