#include <stdio.h>
#include <string.h>
void insert(char a[], int pos, int s, char k)
{
    a[strlen(a) + s] = 0;
    for (int i = strlen(a) - 1 + s; i >= s + pos; i--)
        a[i] = a[i - s];
    for (int i = pos; i < s + pos; i++)
        a[i] = k;
}
void flip(char a[])
{
    char b[1000];
    int n = strlen(a);
    for (int i = n - 1, j = 0; i >= 0, j < n; i--, j++)
    {
        b[j] = a[i];
    }
    b[n] = 0;
    strcpy(a, b);
}
void tru(char a[], char b[])
{
    if (strcmp(a, b) == 0)
    {
        a[0] = '0';
        a[1] = 0;
        return;
    }
    int n = strlen(a), m = strlen(b), temp = 0;
    char s[1000];
    if (n > m)
        insert(b, 0, n - m, '0');
    else if (n < m)
    {
        insert(a, 0, m - n, '0');
        n = m;
    }
    if (strcmp(b, a) > 0)
    {
        char c[1000];
        strcpy(c, a);
        strcpy(a, b);
        strcpy(b, c);
    }
    for (int i = n - 1, j = 0; i >= 0, j < n; i--, j++)
    {
        temp = a[i] - b[i] - temp;
        if (temp < 0)
        {
            temp += 10;
            s[j] = temp + 48;
            temp = 1;
        }
        else
        {
            s[j] = temp + 48;
            temp = 0;
        }
    }
    while (s[n - 1] == '0')
        n--;
    s[n] = 0;
    flip(s);
    strcpy(a, s);
}
int main()
{
    int t;
    scanf("%d\n", &t);
    while (t--)
    {
        char a[1000], b[1000];
        scanf("%s%s", &a, &b);
        tru(a, b);
        printf("%s\n", a);
    }
}
