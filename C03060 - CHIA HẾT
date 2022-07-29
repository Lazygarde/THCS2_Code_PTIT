#include <stdio.h>
int main()
{
    int n, m, k, s = 0;
    scanf("%d%d", &n, &k);
    for (int i = 2; i <= n; i++)
    {
        m = i;
        while (m % 2 == 0)
        {
            s++;
            if (s == k)
                break;
            m /= 2;
        }
        if (s == k)
            break;
    }
    if (s == k)
        printf("Yes");
    else
        printf("No");
}
