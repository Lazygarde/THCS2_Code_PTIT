#include <stdio.h>
int main(){
	int a,b;
	scanf("%d%d",&a,&b);
	for(int i=a;i<b;i++){
		for(int j=i+1;j<=b;j++){
			int m=i,n=j;
			while(m!=n){
				if(m>n) m-=n;
				else n-=m;
			}
			if(n==1) printf("(%d,%d)\n",i,j);
		}
	}
}
