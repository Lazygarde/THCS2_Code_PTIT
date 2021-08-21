#include <stdio.h>
int main(){
	int m,n,k;
	scanf("%d%d",&m,&n);
	if(m<=n){
		int h=n;
		for(int i=0;i<m;i++){
			k=0;
			for(int j=h;j>=1;j--){
				k++;
				printf("%d",j);
			}
			for(int j=2;j<2+(n-k);j++){
				printf("%d",j);
			}
			h--;
			printf("\n");
		}
	}
	else{
		int h=m;
		for(int i=n;i<m;i++){
			for(int j=h;j>h-n;j--){
				printf("%d",j);
			}
			h--;
			printf("\n");
		}
		for(int i=0;i<n;i++){
			k=0;
			for(int j=h;j>=1;j--){
				k++;
				printf("%d",j);
			}
			for(int j=2;j<2+(n-k);j++){
				printf("%d",j);
			}
			h--;
			printf("\n");
		}
		
	}
}
