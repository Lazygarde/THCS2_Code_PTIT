#include <stdio.h>
#include <math.h>
int main(){
	int t;
	scanf("%d",&t);
	for(int k=1;k<=t;k++){
		int n;
		scanf("%d",&n);
		printf("Test %d: ",k);
		for(int i=2;i<=sqrt(n);i++){
			int s=0;
			while(n%i==0){
				s++;
				n/=i;
			}
			if(s>0) printf("%d(%d) ",i,s);
		}
		if(n>1) printf("%d(1)",n);
		printf("\n");
	}
}
