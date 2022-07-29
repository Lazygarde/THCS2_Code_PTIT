#include <stdio.h>
void swap(int *a, int *b)
{
    int c = *a;
    *a = *b;
    *b = c;
}
int main()
{
    int z[6], k, a, b, c, d, e, f;
    for (int i = 0; i < 6; i++)
        scanf("%d", &z[i]);
    for (int i = 0; i < 6; i += 2)
        if (z[i + 1] > z[i])
            swap(&z[i], &z[i + 1]);
    for (int i = 0; i < 4; i += 2)
    {
        for (int j = i + 2; j < 6; j += 2)
        {
            if (z[j] > z[i])
            {
                swap(&z[i], &z[j]);
                swap(&z[i + 1], &z[j + 1]);
            }
        }
    }
    if (z[0] == z[2] && z[2] == z[4] && z[0] == z[1] + z[3] + z[5])
    {
        printf("YES");
        return 0;
    }
    for (int i = 0; i < 2; i++)
    {
        if (i == 0)
        {
            a = z[0];
            b = z[1];
        }
        else
        {
            a = z[1];
            b = z[0];
        }
        for (int j = 0; j < 2; j++)
        {
            if (j == 0)
            {
                c = z[2];
                d = z[3];
            }
            else
            {
                c = z[3];
                d = z[2];
            }
            for (int y = 0; y < 2; y++)
            {
                if (y == 0)
                {
                    e = z[4];
                    f = z[5];
                }
                else
                {
                    e = z[5];
                    f = z[4];
                }
                if (a == f + d && e == c && b + c == a)
                {
                    printf("YES");
                    return 0;
                }
            }
        }
    }
    printf("NO");
}
