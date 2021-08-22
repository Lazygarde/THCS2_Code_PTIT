#include <stdio.h>
int nto(int n){
    if(n<2) return 0;
    for(int i=2;i*i<=n;i++){
        if(n%i==0) return 0;
    }
    return 1;
}
int main(){
	int t;
	scanf("%d",&t);
	while(t--){
		int n;
		scanf("%d",&n);
		if(nto(n)) printf("YES\n");
		else printf("NO\n");
	}
}
