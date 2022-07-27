#include <stdio.h>
int n;
void swap(int a[], int b[])
{
    for (int i = 1; i <= n; i++)
    {
        int c = a[i];
        a[i] = b[i];
        b[i] = c;
    }
}
int main()
{
    scanf("%d", &n);
    int a[n + 2], b[n + 2];
    a[0] = 0;
    a[1] = 1;
    for (int i = 2; i <= n + 1; i++)
    {
        for (int j = 1; j < i; j++)
        {
            b[j] = a[j] + a[j - 1];
            printf("%d ", a[j]);
        }
        b[i] = 1;
        printf("\n");
        swap(a, b);
    }
}
