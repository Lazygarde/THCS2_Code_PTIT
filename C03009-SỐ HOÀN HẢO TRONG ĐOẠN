#include <stdio.h>
int main(){
	int a,b;
	scanf("%d%d",&a,&b);
	if(a>b){
		int c=a;
		a=b;
		b=c;
	}
	if(a>496){
	    if(b>=8128) printf("8128");
	}
	else if(a>28){
		if(b>=8128) printf("496 8128");
		else if(b>=496) printf("496");
	}
	else if(a>6){
		if(b>=8128) printf("28 496 8128");
		else if(b>=496) printf("28 496");
		else if(b>=28) printf("28");
	}
	else if(a>=1){
		if(b>=8128) printf("6 28 496 8128");
		else if(b>=496) printf("6 28 496");
		else if(b>=28) printf("6 28");
		else if(b>=6) printf("6");
	}
}
