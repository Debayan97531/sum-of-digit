#include <stdio.h>
int sum(int );
int main()
{
    int num,result;
    printf("enter any number:");
    scanf("%d",&num);
    result=sum(num);
    printf("sum of digit is %d\n",result);
}
int sum(int num)
{
    if(num>0)
    {
        return(num%10+sum(num/10));
    }
}
