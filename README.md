# Armstrong-no-if-else-c-programming-language
This program is check whether a given no  is Armstrong or not using if-else.
#include<stdio.h>
#include<conio.h>
int main()
{
    int num,Lastdigit,sum=0,temp;
    printf("enter your no:-\n");
    scanf("%d",&num);
    temp=num;
    while(num>0)
    {
	     Lastdigit=num%10;
	     sum=sum+(Lastdigit*Lastdigit*Lastdigit);
	     num=num/10;
    }
    if(temp==sum)
    printf("%d is a armstrong no.",temp);
    else
    printf("%d is not a armstrong no.",temp);
    getch();
    return 0;
}
