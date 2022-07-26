#include <stdio.h>
#include <math.h>
struct Triangle
{
    float a, b, c;
    float p;
    float S;
};
int main()
{
    int n;
    scanf("%d", &n);
    struct Triangle k, f[n + 1];
    for (int i = 1; i <= n; i++)
    {
        scanf("%f%f%f", &f[i].a, &f[i].b, &f[i].c);
        f[i].p = (f[i].a + f[i].b + f[i].c) * 0.5;
    }
    for (int i = 1; i <= n; i++)
        f[i].S = sqrt(f[i].p * (f[i].p - f[i].a) * (f[i].p - f[i].b) * (f[i].p - f[i].c));
    for (int i = 1; i < n; i++)
    {
        for (int j = n; j > i; j--)
        {
            if (f[j].S < f[j - 1].S)
            {
                k = f[j];
                f[j] = f[j - 1];
                f[j - 1] = k;
            }
        }
    }
    for (int i = 1; i <= n; i++)
        printf("%1.f %1.f %1.f\n", f[i].a, f[i].b, f[i].c);
}
