#include <stdio.h>
int main()
{
    int n;
    scanf("%d", &n);
    int a[n];
    for (int i = 0; i < n; i++)
        scanf("%d", &a[i]);
    for (int i = n - 1; i >= 0; i--)
    {
        int s = 0;
        for (int j = 0; j < i; j++)
        {
            if (a[j + 1] < a[j])
            {
                int k = a[j + 1];
                a[j + 1] = a[j];
                a[j] = k;
            }
            else
                s++;
        }
        if (s == i)
            return 0;
        printf("Buoc %d: ", n - i);
        for (int j = 0; j < n; j++)
            printf("%d ", a[j]);
        printf("\n");
    }
}
