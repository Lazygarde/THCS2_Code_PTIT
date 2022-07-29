#include <stdio.h>
#include <math.h>
void swap(int *a, int *b)
{
    int c = *a;
    *a = *b;
    *b = c;
}
int main()
{
    int a[4], b[4];
    for (int i = 0; i < 4; i++)
        scanf("%d%d", &a[i], &b[i]);
    for (int i = 0; i < 4; i++)
        for (int j = 3; j > i; j--)
            if (a[j] < a[j - 1])
                swap(&a[j], &a[j - 1]);
    int x1 = abs(a[3] - a[0]);
    for (int i = 0; i < 3; i++)
        for (int j = 3; j > i; j--)
            if (b[j] < b[j - 1])
                swap(&b[j], &b[j - 1]);
    int x2 = abs(b[3] - b[0]);
    if (x1 > x2)
        printf("%d", x1 * x1);
    else
        printf("%d", x2 * x2);
}
