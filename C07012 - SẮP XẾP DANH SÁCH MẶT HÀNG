#include <stdio.h>
#include <string.h>
struct Item
{
    int id;
    char name[100];
    char group[100];
    double buyPrice;
    double sellPrice;
    double profit;
};
int cmp(struct Item a, struct Item b)
{
    if (a.profit < b.profit)
        return 1;
    return 0;
}
void swap(struct Item *a, struct Item *b)
{
    struct Item c = *a;
    *a = *b;
    *b = c;
}
int main()
{
    int n;
    scanf("%d", &n);
    struct Item a[n + 1];
    for (int i = 1; i <= n; i++)
    {
        scanf("\n");
        a[i].id = i;
        gets(a[i].name);
        gets(a[i].group);
        scanf("%lf%lf", &a[i].buyPrice, &a[i].sellPrice);
        a[i].profit = a[i].sellPrice - a[i].buyPrice;
    }
    for (int i = 1; i <= n; i++)
        for (int j = i + 1; j <= n; j++)
            if (cmp(a[i], a[j]))
                swap(&a[i], &a[j]);
    for (int i = 1; i <= n; i++)
    {
        printf("%d %s %s %.2lf\n", a[i].id, a[i].name, a[i].group, a[i].profit);
    }
}
