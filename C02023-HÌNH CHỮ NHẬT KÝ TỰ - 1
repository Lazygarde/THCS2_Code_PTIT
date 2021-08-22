#include <stdio.h>
int main(){
	int m,n;
	scanf("%d%d",&m,&n);
	if(m<=n){
		char x='a'+n-1,y='a'+n-1;
		int k=1;
		for(int i=0;i<m;i++){
			for(int j=0;j<k;j++){
				printf("%c",x-j);
			}
			for(int j=k;j<n;j++){
				printf("%c",y);
			}
			y--;
			k++;
			printf("\n");
		}
	}
	else{
		char x='a'+m-1,y='a'+m-1;
		int k=1;
		for(int i=0;i<n;i++){
			for(int j=0;j<k;j++){
				printf("%c",x-j);
			}
			for(int j=k;j<n;j++){
				printf("%c",y);
			}
			y--;
			k++;
			printf("\n");
		}
		for(int i=n;i<m;i++){
			y='a'+m-1;
			for(int j=0;j<n;j++){
				printf("%c",y);
				y--;
			}
			printf("\n");
		}
	}
}
