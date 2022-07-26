#include <stdio.h>
#include <string.h>
int cmp(char a[], char b[])
{
    char c[500], d[500];
    strcpy(c, a);
    strcpy(d, b);
    strcat(c, b);
    strcat(d, a);
    if (strcmp(c, d) > 0)
        return 1;
    return 0;
}
void swap(char a[], char b[])
{
    char c[200];
    strcpy(c, a);
    strcpy(a, b);
    strcpy(b, c);
}
int main()
{
    int t;
    scanf("%d", &t);
    while (t--)
    {
        int n;
        scanf("%d", &n);
        char a[100][200];
        for (int i = 0; i < n; i++)
            scanf("%s", a[i]);
        for (int i = 0; i < n; i++)
            for (int j = i + 1; j < n; j++)
                if (cmp(a[i], a[j]))
                    swap(a[i], a[j]);
        for (int i = 0; i < n; i++)
            printf("%s", a[i]);
        printf("\n");
    }
}
