#include <stdio.h>
#include <string.h>
int main()
{
    int t;
    scanf("%d\n", &t);
    while (t--)
    {
        char a[20];
        scanf("%s", a);
        int n = strlen(a);
        long long s = 0;
        for (int i = 0; i < n; i++)
        {
            if (a[i] == '0' || a[i] == '8' || a[i] == '9')
                s = s * 10;
            else if (a[i] == '1')
                s = s * 10 + 1;
            else
            {
                s = -1;
                break;
            }
        }
        if (s > 0)
            printf("%lld\n", s);
        else
            printf("INVALID\n");
    }
}
