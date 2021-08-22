#include <stdio.h>
#include <string.h>
int main(){
	char a[100000];
	gets(a);
	int n=strlen(a),x=0,y=0,z=0;
	for(int i=0;i<n;i++){
		if(a[i]>=65&&a[i]<=90) x++;
		else if(a[i]>=97&&a[i]<=122) x++;
		else if(a[i]>=48&&a[i]<=57) y++;
		else z++;
	}
	printf("%d %d %d",x,y,z);
}
