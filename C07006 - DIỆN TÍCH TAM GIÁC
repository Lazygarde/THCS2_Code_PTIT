#include <stdio.h>
#include <math.h>
int check(double a, double b, double c)
{
    if (a == 0 || b == 0 || c == 0)
        return 0;
    if (a + b <= c || a + c <= b || b + c <= a)
        return 0;
    return 1;
}
int main()
{
    int t;
    scanf("%d", &t);
    while (t--)
    {
        double a, b, c, d, e, f;
        scanf("%lf%lf%lf%lf%lf%lf", &a, &b, &c, &d, &e, &f);
        double x = sqrt((a - c) * (a - c) + (b - d) * (b - d));
        double y = sqrt((a - e) * (a - e) + (b - f) * (b - f));
        double z = sqrt((e - c) * (e - c) + (f - d) * (f - d));
        if (check(x, y, z) == 0)
            printf("INVALID\n");
        else
        {
            double p = (x + y + z) / 2.0;
            double s = sqrt(p * (p - x) * (p - y) * (p - z));
            printf("%0.2lf\n", s);
        }
    }
}
