#include <stdio.h>
#include <string.h>
int main()
{
    int t;
    scanf("%d\n", &t);
    while (t--)
    {
        char a[100];
        gets(a);
        int s = 1, n = strlen(a);
        for (int i = 1; i < n; i++)
            if (a[i] != ' ' && a[i - 1] == ' ')
                s++;
        printf("%d\n", s);
    }
}
