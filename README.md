#include<stdio.h>

int main(void)
{
    int arr[100];

    int i,n,j,k,temp;

    while(scanf("%d",&n)!=EOF){

    for(i=1;i<=n;i++)
        scanf("%d",&arr[i]);

    for(i=1;i<=n-1;i++)
    {
        for(j=i+1;j<=n;j++)
        {
            if(arr[i]>arr[j])
            {
                temp=arr[i];
                arr[i]=arr[j];
                arr[j]=temp;
            }

            }
        }
        for(k=1;k<=n;k++)

            printf("%d ",arr[k]);

            printf("\n");


    }
    return 0;
}

