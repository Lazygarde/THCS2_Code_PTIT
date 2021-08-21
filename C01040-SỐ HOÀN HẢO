#include <stdio.h>
#include <math.h>
int main(){
	int n;
	scanf("%d",&n);
	int ok=1;
	if(n==0||n==1) ok=0;
	long long s=1;
	for(int i=2;i<sqrt(n);i++){
		if(n%i==0) s=s+i+n/i;
	}
	if(sqrt(n)==(int)sqrt(n)) s+=sqrt(n);
	if(s!=n) ok=0;
	printf("%d",ok);
}
