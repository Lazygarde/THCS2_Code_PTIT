#include <stdio.h>
int main(){
	int n;
	scanf("%d",&n);
	int a[n],b[100001]={};
	for(int i=0;i<n;i++){
		scanf("%d",&a[i]);
		b[a[i]]++;
	}
	int s=0;
	for(int i=0;i<n;i++){
		if(b[a[i]]==1) s++;
	}
	printf("%d\n",s);
	for(int i=0;i<n;i++){
		if(b[a[i]]==1) printf("%d ",a[i]);
	}
}
