#include <stdio.h>
struct PhanSo
{
    int tuSo, mauSo;
};
int gcd(int a, int b)
{
    while (a != 0)
    {
        int x = a;
        a = b % a;
        b = x;
    }
    return b;
}
int lcm(int a, int b)
{
    return a * b / gcd(a, b);
}
int main()
{
    int t;
    scanf("%d", &t);
    for (int z = 1; z <= t; z++)
    {
        struct PhanSo a, b, c, d;
        scanf("%d%d%d%d", &a.tuSo, &a.mauSo, &b.tuSo, &b.mauSo);
        printf("Case #%d:\n", z);
        int x = gcd(a.tuSo, a.mauSo);
        a.tuSo /= x;
        a.mauSo /= x;
        x = gcd(b.tuSo, b.mauSo);
        b.tuSo /= x;
        b.mauSo /= x;
        int k = lcm(a.mauSo, b.mauSo);
        a.tuSo *= k / a.mauSo;
        b.tuSo *= k / b.mauSo;
        a.mauSo = b.mauSo = k;
        printf("%d/%d %d/%d\n", a.tuSo, a.mauSo, b.tuSo, b.mauSo);
        c.tuSo = a.tuSo + b.tuSo;
        c.mauSo = k;
        x = gcd(c.tuSo, c.mauSo);
        c.tuSo /= x;
        c.mauSo /= x;
        printf("%d/%d\n", c.tuSo, c.mauSo);
        c.tuSo = a.tuSo * b.mauSo;
        c.mauSo = a.mauSo * b.tuSo;
        x = gcd(c.tuSo, c.mauSo);
        c.tuSo /= x;
        c.mauSo /= x;
        printf("%d/%d\n", c.tuSo, c.mauSo);
    }
}
