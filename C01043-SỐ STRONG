#include <stdio.h>
int main(){
	int n,s=0;
	scanf("%d",&n);
	int c=n;
	while(c!=0){
		int b=c%10;
		int d=1;
		for(int i=1;i<=b;i++) d*=i;
		s+=d;
		if(s>n) break;
		c/=10;
	}
	if(s==n) printf("1");
	else printf("0");
}
