#include <stdio.h>
struct data
{
    int nm, id;
};
void qsort(struct data a[], int l, int r)
{
    int i = l, j = r, k = a[(l + r) / 2].nm;
    while (i <= j)
    {
        while (a[i].nm < k)
            i++;
        while (a[j].nm > k)
            j--;
        if (i <= j)
        {
            struct data k = a[i];
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
        int n, ans, min = 1e9;
        scanf("%d", &n);
        struct data a[n];
        for (int i = 0; i < n; i++)
        {
            a[i].id = i;
            scanf("%d", &a[i].nm);
        }
        qsort(a, 0, n - 1);
        for (int i = 1; i < n; i++)
        {
            if (a[i].nm == a[i - 1].nm)
            {
                if (a[i].id < min)
                {
                    min = a[i].id;
                    ans = a[i].nm;
                }
                if (a[i - 1].id < min)
                {
                    min = a[i - 1].id;
                    ans = a[i - 1].nm;
                }
            }
        }
        if (min != 1e9)
            printf("%d\n", ans);
        else
            printf("NO\n");
    }
}
