#include <stdio.h>
#include <string.h>
int main(){
	char s2[200],a[100][100],k;
	int pos1=0;
	while(scanf("%s",&a[pos1])!=-1){
		pos1++;
		k=getchar();
		if(k==10) break;
	}
	gets(s2);
	for(int i=0;i<pos1;i++){
		if(strcmp(a[i],s2)==0){
			a[i][0]=0;
		}
		if(a[i][0]!=0) printf("%s ",a[i]);
	}
}
