#include <stdio.h>
int main(){
	int n;
	scanf("%d",&n);
	int a[n];
	for(int i=0;i<n;i++) scanf("%d",&a[i]);
	int pos,x;
	for(int i=1;i<n;i++){
		x=a[i]; 
		pos=i;
		while(pos>0&&x<a[pos-1]){
			a[pos]=a[pos-1];
			pos--;
		}
		a[pos]=x;
	}
	for(int i=0;i<n;i++) printf("%d ",a[i]);
}
