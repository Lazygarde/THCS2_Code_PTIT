#include <stdio.h>
int nto(int n){
	if(n<2) return 0;
	for(int i=2;i*i<=n;i++){
		if(n%i==0) return 0;
	}
	return 1;
}
int fibo(int n){
	int a=1,b=1;
	while(a<n){
		int c=a+b;
		b=a;
		a=c;
	}
	if(a==n) return 1;
	return 0;
}
int tfibo(int n){
	int s=0;
	while(n!=0){
		s+=n%10;
		n/=10;
	}
	if(fibo(s)) return 1;
	return 0;
}
int main(){
	int a,b;
	scanf("%d%d",&a,&b);
	if(a>b){
		int c=a;
		a=b;
		b=c;
	}
	for(int i=a;i<=b;i++){
		if(nto(i)&&tfibo(i)) printf("%d ",i);
	}
}
