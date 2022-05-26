# Project-Euler-2-Even-Fibonacci-numbers
#include <math.h>

#include <stdio.h>

#include <string.h>

#include <stdlib.h>

#include <assert.h>

#include <limits.h>

#include <stdbool.h>


int main(){
    
    int t; 
    scanf("%d",&t);
    
    for(int a0 = 0; a0 < t; a0++){
        long n; 
        scanf("%ld",&n);
        long a=2,b=8,t=0,s=0;
        while(a<n){
            s+=a;
            t=b;
            b=4*b+a;
            a=t;
        }
        printf("%ld\n",s);
    }
    return 0;
}
