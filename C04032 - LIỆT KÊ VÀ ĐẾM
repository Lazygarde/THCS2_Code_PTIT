#include <stdio.h>
struct data
{
    int nm, s;
};
int check(int n)
{
    int x = 9;
    while (n != 0)
    {
        int k = n % 10;
        if (k > x)
            return 0;
        x = k;
        n /= 10;
    }
    return 1;
}
int cmp(struct data a, struct data b)
{
    if (a.s < b.s)
        return 1;
    return 0;
}
void swap(struct data *a, struct data *b)
{
    struct data c = *a;
    *a = *b;
    *b = c;
}
int main()
{
    struct data a[100000];
    int x, n = 0;
    while (scanf("%d", &x) != -1)
    {
        if (check(x))
        {
            int ok = 0;
            for (int i = 0; i < n; i++)
            {
                if (a[i].nm == x)
                {
                    ok = 1;
                    a[i].s++;
                    break;
                }
            }
            if (!ok)
            {
                a[n].nm = x;
                a[n].s = 1;
                n++;
            }
        }
    }
    for (int i = 0; i < n; i++)
        for (int j = i + 1; j < n; j++)
            if (cmp(a[i], a[j]))
                swap(&a[i], &a[j]);
    for (int i = 0; i < n; i++)
        printf("%d %d\n", a[i].nm, a[i].s);
}
