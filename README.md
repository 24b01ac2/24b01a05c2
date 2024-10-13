1) c program to convert farenheit to celsius
#include <stdio.h>
 int main()
{
    
    float f,c;
    printf("enter the value f:");
    scanf("%f",&f);
    c=(f-32)*5.0/9.0;
    printf("%f",c);
    return 0;
}
output: 
   enter the value f:60
15.555555

2) c-program to verify whether or not a given number is palidrome
#include <stdio.h>
int main() 
{
    int num,revnum=0,remainder,originalnum;
    printf("enter the value num:");
    scanf("%d",&num);
    originalnum=num;
    while(num>0)
    {
        remainder=num%10;
        revnum=revnum*10+remainder;
        num=num/10;
    }
    if(originalnum == revnum)
    {
        printf("the palindrome is %d",originalnum);
    }
    else
    {
        printf("not a palindrome %d",originalnum);
    }
    return 0;
}
output:
1)enter the value num:12321
the palindrome is 12321
2)enter the value num:1234
not a palindrome 1234
  
3)write a c-program to input the electricity units and calculate the total electricity bill according to the given conditions:
for first 50units Rs.0.50/unit
for next 100units Rs.0.75/unit
for next 100units Rs.1.20/unit
for above 250units Rs.1.50/unit
#include <stdio.h>
int main() 
{
    int units;
    float bill;
    printf("enter the value if units:");
    scanf("%d",&units);
    if(units<=50)
    {
        bill=units*50;
    }
    else if(units<=150)
    {
        bill=50*0.50+(units-50)*0.75;
    }
    else if(units<=250)
    {
        bill=50*0.50+100*0.75+(units-150)*1.20;
    }
    else
    
        bill=50*0.50+100*0.75+100*1.20+(units-250)*1.50;
    }
    printf("total bill %f",bill);
    return 0;
}
output:
1)enter the value if units:250
total bill 220.000000
2)enter the value if units:300
total bill 295.000000

4)write a c-program to find the largest among the four given numbers using nested if..else



























































