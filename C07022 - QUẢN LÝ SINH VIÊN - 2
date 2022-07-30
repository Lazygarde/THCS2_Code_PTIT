#include <stdio.h>
#include <string.h>
struct Student
{
    int msv;
    char name[100];
    float a, b, c;
    float sum;
};
struct Student f[100];
void add(int n)
{
    int d = 1;
    while (d <= n)
    {
        f[d].msv = d;
        scanf("\n");
        gets(f[d].name);
        scanf("%f%f%f", &f[d].a, &f[d].b, &f[d].c);
        f[d].sum = f[d].a + f[d].b + f[d].c;
        d++;
    }
}
void change(int d)
{
    scanf("\n");
    gets(f[d].name);
    scanf("%f%f%f", &f[d].a, &f[d].b, &f[d].c);
}
void show(int i)
{
    printf("%d ", f[i].msv);
    printf("%s ", f[i].name);
    printf("%.1f %.1f %.1f\n", f[i].a, f[i].b, f[i].c);
}
void check(int n)
{
    for (int i = 1; i <= n; i++)
        if (f[i].a < f[i].b && f[i].b < f[i].c)
            show(i);
}
int main()
{
    int n;
    while (1)
    {
        int x = 0;
        scanf("%d", &x);
        if (x == 1)
        {
            scanf("%d\n", &n);
            add(n);
            printf("%d\n", n);
        }
        else if (x == 2)
        {
            int m;
            scanf("%d", &m);
            change(m);
            printf("%d\n", m);
        }
        else
        {
            check(n);
            return 0;
        }
    }
}
