#include <stdio.h>
int main(){
	int m,n,k=0,h;
	scanf("%d%d",&m,&n);
	if(m<=n){
		for(int i=1;i<=m;i++){
			h=0;
			for(int j=k;j<n;j++){
				h++;
				printf("%d",j+1);
			}
			for(int j=n-1;j>=h;j--){
				printf("%d",j);
			}
			k++;
			printf("\n");
		}
	}
	else{
		for(int i=1;i<=n;i++){
			h=0;
			for(int j=k;j<n;j++){
				h++;
				printf("%d",j+1);
			}
			for(int j=n-1;j>=h;j--){
				printf("%d",j);
			}
			k++;
			printf("\n");
		}
		for(int i=n;i<m;i++){
			printf("%d",i+1);
			for(int j=i;j>i-(n-1);j--){
				printf("%d",j);
			}
			printf("\n");
		}
	}
}
