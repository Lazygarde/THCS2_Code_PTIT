#include <stdio.h>
#include <math.h>
int check(float a, float b, float c)
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
        float a, b, c, d, e, f;
        scanf("%f%f%f%f%f%f", &a, &b, &c, &d, &e, &f);
        float x = sqrt((a - c) * (a - c) + (b - d) * (b - d));
        float y = sqrt((a - e) * (a - e) + (b - f) * (b - f));
        float z = sqrt((e - c) * (e - c) + (f - d) * (f - d));
        if (check(x, y, z) == 0)
            printf("INVALID\n");
        else
            printf("%0.3f\n", x + y + z);
    }
}
