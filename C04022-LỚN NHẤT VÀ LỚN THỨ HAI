#include <stdio.h>
int main(){
	int n;
	scanf("%d",&n);
	int a[n];
	for(int i=0;i<n;i++) scanf("%d",&a[i]);
	int m=0,k=0;
	for(int i=0;i<n;i++) if(a[i]>k) k=a[i];
	for(int i=0;i<n;i++) if(a[i]>m&&a[i]!=k) m=a[i];
	printf("%d %d",k,m);
}
