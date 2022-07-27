#include <stdio.h>
int main()
{
    int n;
    scanf("%d", &n);
    int a[n];
    for (int i = 0; i < n; i++)
        scanf("%d", &a[i]);
    for (int i = 0; i < n - 1; i++)
    {
        for (int j = i + 1; j < n; j++)
        {
            if (a[i] > a[j])
            {
                int k = a[j];
                a[j] = a[i];
                a[i] = k;
            }
        }
        printf("Buoc %d: ", i + 1);
        for (int j = 0; j < n; j++)
            printf("%d ", a[j]);
        printf("\n");
    }
}
