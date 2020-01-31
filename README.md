#include <stdio.h>

int main()
{
    int n,a[10],i,t,j;
    float avg;
    printf("enter the number:");
    scanf("%d",&n);
    for(i=0;i<n;i++)
    {
        scanf("%d",&a[i]);
    }
    
    for(i=0;i<n-1;i++)
    {
        for(j=0;j<n;j++)
        {
            if(a[i]>a[j+1])
            {
                t=a[i];
                a[i]=a[j];
                a[j]=t;
            }
        }
        
        
    }
    for(i=0;i<n;i++)
    {
       printf("%d",a[i]); 
    }
    return 0;
}
output:enter the number:3
3
2
4
234
