#include <stdio.h>
void qsort(int a[], int l, int r)
{
    int i = l, j = r;
    int k = a[(l + r) / 2];
    while (i <= j)
    {
        while (a[i] < k)
            i++;
        while (a[j] > k)
            j--;
        if (i <= j)
        {
            int m = a[i];
            a[i] = a[j];
            a[j] = m;
            i++;
            j--;
        }
    }
    if (l < j)
        qsort(a, l, j);
    if (i < r)
        qsort(a, i, r);
}
void in(int a[], int n)
{
    for (int i = 0; i < n; i++)
        printf("%d ", a[i]);
}
int main()
{
    int n;
    scanf("%d", &n);
    int x, b[n], c[n], nb = 0, nc = 0;
    for (int i = 0; i < n; i++)
    {
        scanf("%d", &x);
        if (x % 2 == 0)
            b[nb++] = x;
        else
            c[nc++] = x;
    }
    qsort(b, 0, nb - 1);
    qsort(c, 0, nc - 1);
    in(b, nb);
    in(c, nc);
}
