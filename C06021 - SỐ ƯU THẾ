#include <stdio.h>
#include <string.h>
int check(char a[])
{
    int n = strlen(a);
    if (a[0] == '0')
        return -1;
    int sc = 0, sl = 0, d = 0;
    for (int i = 0; i < n; i++)
    {
        if (a[i] == '0' || a[i] == '2' || a[i] == '4' || a[i] == '6' || a[i] == '8')
        {
            sc++;
            d++;
        }
        else if (a[i] == '1' || a[i] == '3' || a[i] == '5' || a[i] == '7' || a[i] == '9')
        {
            sl++;
            d++;
        }
        else
            return -1;
    }
    if (sc > sl && n % 2 == 0)
        return 1;
    if (sl > sc && n % 2 != 0)
        return 1;
    return 0;
}
int main()
{
    int t;
    scanf("%d", &t);
    while (t--)
    {
        char a[1005];
        scanf("%s", a);
        int k = check(a);
        if (k == 1)
            printf("YES\n");
        else if (k == 0)
            printf("NO\n");
        else
            printf("INVALID\n");
    }
}
