#include <stdio.h>
#include <string.h>
int main()
{
    char s[60];
    scanf("%s", &s);
    int d = 0, a[26], b[26];
    for (int i = 0; i < 26; i++)
        a[i] = -1;
    for (int i = 0; i < 52; i++)
    {
        if (a[s[i] - 'A'] == -1)
            a[s[i] - 'A'] = i;
        else
            b[s[i] - 'A'] = i;
    }
    for (int i = 0; i < 26; i++)
        for (int j = 0; j < 26; j++)
            if (a[i] < a[j] && a[j] < b[i] && b[i] < b[j])
                d++;
    printf("%d", d);
}
