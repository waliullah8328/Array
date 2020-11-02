#include<stdio.h>
int main()
{
int i,j,n,k,ary[100];
  scanf("%d",&n);
  for(i=0;i<n;i++){
    scanf("%d",&ary[i]);
  }

  for(i=0;i<n;i++){
    for(j=0;j<n-1;j++){
      if(ary[j]<ary[j+1]){
        k=ary[j];
        ary[j]=ary[j+1];
        ary[j+1]=k;
      }
    }
  }
printf("Elder one will get = %d\n",ary[0]);
printf("Younge one will get= %d",ary[1]);
    return 0;
}

