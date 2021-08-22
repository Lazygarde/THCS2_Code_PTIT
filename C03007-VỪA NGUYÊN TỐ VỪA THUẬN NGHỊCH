#include <stdio.h>
#include <math.h>
int main(){
	int t;
	scanf("%d",&t);
	while(t--){
		int a,b;
		scanf("%d%d",&a,&b);
		int k=0;
		for(int i=a;i<=b;i++){
			int ok=1,c=i,s=0;
			while(c!=0){
				s=s*10+c%10;
				c/=10;
			}
			if(s==i){
				for(int j=2;j<=sqrt(i);j++){
					if(i%j==0){
						ok=0;
						break;
					}
				}
			}
			else ok=0;
			if(ok==1){
				printf("%d ",i);
				k++;
			}
			if(k==10){
				printf("\n");
				k=0;
			}
		}
		printf("\n\n");
	}
}
