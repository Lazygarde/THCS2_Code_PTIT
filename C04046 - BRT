#include <stdio.h>
#include <math.h>
void qsort(long long a[], int l, int r)
{
    int i = l, j = r;
    long long k = a[(l + r) / 2];
    while (i <= j)
    {
        while (a[i] < k)
            i++;
        while (a[j] > k)
            j--;
        if (i <= j)
        {
            long long k = a[i];
            a[i] = a[j];
            a[j] = k;
            i++;
            j--;
        }
    }
    if (l < j)
        qsort(a, l, j);
    if (i < r)
        qsort(a, i, r);
}
int main()
{
    int t;
    scanf("%d", &t);
    while (t--)
    {
        int n, s = 0;
        scanf("%d", &n);
        long long a[n + 1], b[n + 1], min = 1e9;
        for (int i = 1; i <= n; i++)
            scanf("%lld", &a[i]);
        qsort(a, 1, n);
        for (int i = 2; i <= n; i++)
        {
            b[i] = abs(a[i] - a[i - 1]);
            if (b[i] < min)
                min = b[i];
        }
        for (int i = 2; i <= n; i++)
            if (b[i] == min)
                s++;
        printf("%lld %d\n", min, s);
    }
}
