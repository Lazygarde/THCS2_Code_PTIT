#include <stdio.h>
int a[100005];
void era()
{
    a[1] = 1;
    for (int i = 2; i * i <= 100000; i++)
        if (!a[i])
            for (int j = i * i; j <= 100000; j += i)
                a[j] = 1;
}
int check(int n)
{
    int s = 0;
    while (n != 0)
    {
        s += n % 10;
        n /= 10;
    }
    if (s % 5 == 0)
        return 1;
    return 0;
}
int main()
{
    era();
    int n, s = 0;
    scanf("%d", &n);
    for (int i = 2; i < n; i++)
    {
        if (!a[i] && check(i))
        {
            s++;
            printf("%d ", i);
        }
    }
    printf("\n%d", s);
}
