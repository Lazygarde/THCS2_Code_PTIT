#include <stdio.h>
int main(){
	int n;
	scanf("%d",&n);
	int a[n],b[100001]={},s=0,c[n];
	for(int i=0;i<n;i++){
		scanf("%d",&a[i]);
		b[a[i]]++;
	}
	for(int i=0;i<n;i++){
		if(b[a[i]]>1){
		    c[s++]=a[i];
		    b[a[i]]=1;
		}
	}
	printf("%d\n",s);
	for(int i=0;i<s;i++) printf("%d ",c[i]);
}
