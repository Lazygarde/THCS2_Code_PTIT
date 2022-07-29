#include <stdio.h>
#include <string.h>
struct Student
{
    int id;
    char name[100];
    char date[100];
    double mark1;
    double mark2;
    double mark3;
    double marksum;
};
int cmp(struct Student a, struct Student b)
{
    if (a.marksum < b.marksum)
        return 1;
    return 0;
}
void swap(struct Student *a, struct Student *b)
{
    struct Student c = *a;
    *a = *b;
    *b = c;
}
int main()
{
    int n;
    scanf("%d", &n);
    double max = 0;
    struct Student a[n + 1];
    for (int i = 1; i <= n; i++)
    {
        scanf("\n");
        a[i].id = i;
        gets(a[i].name);
        gets(a[i].date);
        scanf("%lf%lf%lf", &a[i].mark1, &a[i].mark2, &a[i].mark3);
        a[i].marksum = a[i].mark1 + a[i].mark2 + a[i].mark3;
        if (max < a[i].marksum)
            max = a[i].marksum;
    }
    for (int i = 1; i <= n; i++)
        for (int j = i + 1; j <= n; j++)
            if (cmp(a[i], a[j]))
                swap(&a[i], &a[j]);
    for (int i = 1; i <= n; i++)
        printf("%d %s %s %.1lf\n", a[i].id, a[i].name, a[i].date, a[i].marksum);
}
