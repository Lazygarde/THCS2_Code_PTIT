#include <stdio.h>
int main(){
	int n,m;
	scanf("%d%d",&n,&m);
	if(n<=m){
		char x='A'+n-1;
		int k=m-n;
		for(int j=0;j<n;j++){
			for(int i=0;i<k;i++){
				printf("%c",x+i);
			}
			for(int i=k;i<m;i++){
				printf("%c",'A'+m-1);
			}
			k++;
			x--;
			printf("\n");
		}
	}
	else{
		for(int j=0;j<n-m;j++){
			for(int i=0;i<m;i++){
				printf("%c",'A'+m-1);
			}
			printf("\n");
		}
		char x='A'+m-1;
		int k=0;
		for(int j=n-m;j<n;j++){
			for(int i=0;i<k;i++){
				printf("%c",x+i);
			}
			for(int i=k;i<m;i++){
				printf("%c",'A'+m-1);
			}
			x--;
			k++;
			printf("\n");
		}
	}
}
