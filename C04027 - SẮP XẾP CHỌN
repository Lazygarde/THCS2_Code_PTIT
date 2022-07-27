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
        int p = i;
        for (int j = i + 1; j < n; j++)
            if (a[p] > a[j])
                p = j;
        int k = a[p];
        a[p] = a[i];
        a[i] = k;
        printf("Buoc %d: ", i + 1);
        for (int j = 0; j < n; j++)
            printf("%d ", a[j]);
        printf("\n");
    }
}
