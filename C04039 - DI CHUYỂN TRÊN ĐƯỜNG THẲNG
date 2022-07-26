#include <stdio.h>
#include <math.h>
int main()
{
    int l, r, ans;
    while (scanf("%d%d", &l, &r) != -1)
    {
        int k = abs(r - l);
        if (k == 3)
        {
            printf("3\n");
            continue;
        }
        int x = sqrt(k);
        int n = x * (x - 1);
        if (k - n > 2 * x)
            ans = 2 * x + 1;
        else if (k - n > x)
            ans = 2 * x;
        else
            ans = 2 * x - 1;
        printf("%d\n", ans);
    }
}
