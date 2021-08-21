#include <stdio.h>
int tcs(int n){
    int s=0;
    while(n!=0){
        s+=n%10;
        n/=10;
    }
    return s;
}
int main(){
	int a,b;
	scanf("%d%d",&a,&b);
	if(tcs(a)>tcs(b)) printf("%d %d",b,a);
	else printf("%d %d",a,b);
}
