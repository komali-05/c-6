# c-6
Array program to insert a value
#include<stdio.h>
int main()
{
    int n,i,val,pos;
    printf("enter no.");
    scanf("%d",&n);
    int arr[n+1];
    printf("enter elements");
    for(i=0;i<n;i++)
    {
    scanf("%d",&arr[i]);
    }
    printf("enter inserted element");
    scanf("%d",&val);
    printf("enter the position");
    scanf("%d",&pos);
    for(i=n;i>=pos;i--)
    {
        arr[i]=arr[i-1];
    }
    arr[pos-1]=val;
    n++;
    printf("after insertion:\n");
    for(i=0;i<n;i++)
    {
        printf("%d \t",arr[i]);
    }
    printf("\n");
    return 0;
   }
