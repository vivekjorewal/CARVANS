# CARVANS

#include <stdio.h>

void check(void){
    int n;
    scanf("%d",&n);
    int arr[n];
    for(int i=0;i<n;i++){
        int x;
        scanf("%d",&x);
        arr[i]=x;
    }
    int count = 0;
    // if(n == 0)
    // printf("%d",count);
    // if(n == 1){
    //     printf("%d",1);
    // }
    if(n>1){
    for(int i=0;i<n-1;i++){
        if(arr[i+1]>arr[i]){
            arr[i+1] = arr[i];
            count++;
        }
    }
    }
    printf("%d\n",n-count);
}
int main(void) {
	// your code goes here
	int t;
	scanf("%d",&t);
	for(int i=0;i<t;i++){
	    check();
	}
	return 0;
}
