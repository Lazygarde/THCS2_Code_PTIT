#include <stdio.h>
int tongcso(int n)
{
    int s = 0;
    while (n != 0)
    {
        s += n % 10;
        n /= 10;
    }
    return s;
}
int tongthuasonto(int n)
{
    int s = 0;
    for (int i = 2; i * i <= n; i++)
    {
        while (n % i == 0)
        {
            s += tongcso(i);
            n /= i;
        }
    }
    if (n > 1)
        s += tongcso(n);
    return s;
}
int main()
{
    int n;
    scanf("%d", &n);
    if (tongcso(n) == tongthuasonto(n))
        printf("YES");
    else
        printf("NO");
}
