#include <stdio.h>
void swap(int *a, int *b)
{
    int c = *a;
    *a = *b;
    *b = c;
}
int main()
{
    int t;
    scanf("%d", &t);
    for (int k = 1; k <= t; k++)
    {
        int n;
        scanf("%d", &n);
        int a[n], b[n];
        for (int i = 0; i < n; i++)
            scanf("%d", &a[i]);
        for (int i = 0; i < n; i++)
            scanf("%d", &b[i]);
        for (int i = 0; i < n; i++)
        {
            for (int j = i + 1; j < n; j++)
            {
                if (a[i] > a[j])
                    swap(&a[i], &a[j]);
                if (b[i] < b[j])
                    swap(&b[i], &b[j]);
            }
        }
        printf("Test %d:\n", k);
        for (int i = 0; i < 2 * n; i++)
        {
            if (i % 2 == 0)
                printf("%d ", a[i / 2]);
            else
                printf("%d ", b[(i - 1) / 2]);
        }
        printf("\n");
    }
}
