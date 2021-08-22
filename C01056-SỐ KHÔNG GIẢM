#include <stdio.h>
#include <string.h>
int main(){
	int t;
	scanf("%d\n",&t);
	while(t--){
		char a[20];
		scanf("%s",a);
		int n=strlen(a),ok=0;
		for(int i=1;i<n;i++){
		    if(a[i]<a[i-1]){
		        ok=1;
		        break;
		    }
		}
		if(ok==0) printf("YES\n");
		else printf("NO\n");
	}
}
