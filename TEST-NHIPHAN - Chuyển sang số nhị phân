#include <stdio.h>
int main()
{
    int n, p = 0, a[100];
    scanf("%d", &n);
    if (n == 0)
    {
        printf("0");
        return 0;
    }
    while (n != 0)
    {
        if (n % 2 == 0)
            a[p++] = 0;
        else
            a[p++] = 1;
        n /= 2;
    }
    for (int i = p - 1; i >= 0; i--)
        printf("%d", a[i]);
}
