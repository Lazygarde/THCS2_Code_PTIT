#include <stdio.h>
#include <string.h>
char a[7] = {'I', 'V', 'X', 'L', 'C', 'D', 'M'};
int b[7] = {1, 5, 10, 50, 100, 500, 1000};
int find(char k)
{
    for (int i = 0; i < 7; i++)
        if (a[i] == k)
            return b[i];
    return 0;
}
int main()
{
    int t;
    scanf("%d", &t);
    while (t--)
    {
        char s[100];
        scanf("%s", s);
        int ans = 0, n = strlen(s);
        for (int i = 0; i < n; i++)
        {
            int k1 = find(s[i]), k2 = 0;
            if (i != n - 1)
                k2 = find(s[i + 1]);
            if (k1 < k2)
            {
                ans += k2 - k1;
                i++;
            }
            else
                ans += k1;
        }
        printf("%d\n", ans);
    }
}
