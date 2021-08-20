#include <stdio.h>
int main(){
	int t;
	scanf("%d",&t);
	while(t--){
		int n;
		scanf("%d",&n);
		int a[n],m=-1,b[n],ss=0;
		for(int i=0;i<n;i++) scanf("%d",&a[i]);
		for(int i=n-1;i>=0;i--){
			if(a[i]>m){
				m=a[i];
				b[ss++]=a[i];
			}
		}
		for(int i=ss-1;i>=0;i--) printf("%d ",b[i]);
		printf("\n");
	}
}
