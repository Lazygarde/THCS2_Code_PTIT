#include <stdio.h>
#include <string.h>
int main(){
	char a[102][100],b[100];
	int pos=0;
	while(scanf("%s",&b)!=-1) strcpy(a[pos++],b);
	for(int i=0;i<pos;i++){
		for(int j=i+1;j<pos;j++){
			if(strcmp(a[j],a[i])==0) a[j][0]=0;
		}
		if(a[i][0]!=0) printf("%s ",a[i]);
	}
}
