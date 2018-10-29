#include <stdio.h>
#include <stdlib.h>
#define N 10

void Bubble(int v[], int n)
{
    int i,j,aux;;
    for(i=1; i<=n; i++){
        for(j=0; j<n-i; j++){
            if(v[j]>v[j+1]){
                aux= v[j];
                v[j]= v[j+1];   
                v[j+1]= aux;
            }
        }
    }
}

int main()
{
    int v[] = {5,9,1,4,2,6,7,3,8,10},i;
    Bubble(v,N);
    for (i=0; i<N; i++){
        printf("%d ",v[i]);
    }
}
