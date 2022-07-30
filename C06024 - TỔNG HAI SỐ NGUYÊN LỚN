#include <stdio.h>
#include <string.h>
char a[1000], b[1000];
void insert(char a[], int pos, int s, char k)
{
    a[strlen(a) + s] = 0;
    for (int i = strlen(a) - 1 + s; i >= s + pos; i--)
        a[i] = a[i - s];
    for (int i = pos; i < s + pos; i++)
        a[i] = k;
}
void cong(char a[], char b[])
{
    char s[1000];
    s[0] = 0;
    if (strlen(a) > strlen(b))
        insert(b, 0, strlen(a) - strlen(b), '0');
    else if (strlen(a) < strlen(b))
        insert(a, 0, strlen(b) - strlen(a), '0');
    int tmp = 0;
    for (int i = strlen(a) - 1; i >= 0; i--)
    {
        tmp = a[i] + b[i] - 96 + tmp;
        insert(s, 0, 1, tmp % 10 + 48);
        tmp = tmp / 10;
    }
    if (tmp > 0)
        insert(s, 0, 1, tmp + 48);
    strcpy(a, s);
}
int main()
{
    int t;
    scanf("%d", &t);
    while (t--)
    {
        scanf("%s%s", &a, &b);
        cong(a, b);
        puts(a);
    }
}
