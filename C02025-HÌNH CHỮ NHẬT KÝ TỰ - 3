#include <stdio.h>
int main(){
	int n,m;
	scanf("%d%d",&n,&m);
	printf("@");
	for(int i=0;i<m-1;i++){
		printf("%c",'A'+i);
	}
	printf("\n");
	if(n<=m){
		int k=m-2;
		char f='A';
		for(int i=0;i<n-1;i++){
			for(int j=0;j<k;j++){
				printf("%c",f+j);
			}
			k--;
			f++;
			for(int j=k;j<m-1;j++){
				printf("%c",'A'+m-2);
			}
			printf("\n");
		}
	}
	else{
		int k=m-2;
		char f='A';
		for(int i=0;i<m-1;i++){
			for(int j=0;j<k;j++){
				printf("%c",f+j);
			}
			k--;
			f++;
			for(int j=k;j<m-1;j++){
				printf("%c",'A'+m-2);
			}
			printf("\n");
		}
		for(int i=m-1;i<n-1;i++){
			for(int i=0;i<m;i++){
				printf("%c",'A'+m-2);
			}
			printf("\n");
		}
	}
}
