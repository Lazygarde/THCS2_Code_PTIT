#include <stdio.h>
struct People
{
    int t;
    int d;
};
struct People k, p[10000];
void sort(int n)
{
    for (int i = 1; i <= n; i++)
    {
        for (int j = i + 1; j <= n; j++)
        {
            if (p[i].t > p[j].t)
            {
                k = p[i];
                p[i] = p[j];
                p[j] = k;
            }
        }
    }
}
int main()
{
    int n;
    scanf("%d", &n);
    for (int i = 1; i <= n; i++)
        scanf("%d%d", &p[i].t, &p[i].d);
    sort(n);
    int s = p[1].t;
    p[n + 1].t = 0;
    for (int i = 1; i <= n; i++)
    {
        s += p[i].d;
        if (s < p[i + 1].t)
            s = p[i + 1].t;
    }
    printf("%d", s);
}
