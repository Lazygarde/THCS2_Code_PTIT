#include <stdio.h>
int main(){
	int n;
	scanf("%d",&n);
	int a[n],b[100001]={},c[n],s=0;
	for(int i=0;i<n;i++){
		scanf("%d",&a[i]);
		b[a[i]]++;
		if(b[a[i]]==1){
			c[s]=a[i];
			s++;
		}
	}
	for(int i=0;i<s;i++){
		printf("%d %d\n",c[i],b[c[i]]);
	}
}
