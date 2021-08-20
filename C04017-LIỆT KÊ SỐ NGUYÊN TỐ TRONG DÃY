#include <stdio.h>
int nto(int n){
	if(n<2) return 0;
	for(int i=2;i*i<=n;i++){
		if(n%i==0) return 0;
	}
	return 1;
}
int main(){
	int n,x;
	scanf("%d",&n);
	int a[n],ii=0;
	for(int i=0;i<n;i++){
		scanf("%d",&x);
		if(nto(x)) a[ii++]=x;
	}
	printf("%d ",ii);
	for(int i=0;i<ii;i++) printf("%d ",a[i]);
}
