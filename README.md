1)write a c program to convert farenheit to celsius
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

2)write a c-program to verify whether or not a given number is palidrome
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
 #include <stdio.h>
int main()
{
    int a,b,c,d;
    printf("enter the values of a,b,c,d");
    scanf("%d,%d,%d,%d",&a,&b,&c,&d);
    if(a>b)
    {
        if(a>c)
        {
            if(a>d)
              printf("largest number is %d",a);
            else
              printf("largest number is %d",d);
        }
        else
        {
            if(c>d)
              printf("largest number is %d",c);
            else
              printf("largest number is %d",d);
        }
    }
    else
    {
        if(b>c)
      {
          if(b>d)
            printf("largest number is %d",b);
          else
            printf("largest number is %d",d);
      }
        else
        {
            if(c>d)
              printf("largest number is %d",c);
            else
              printf("largest number is %d",d);
        }
    }
    
    return 0;
}
output:
enter the values of a,b,c,d2,7,5,9
largest number is 9

5)write a c-program to verifty a given number is prime or not
#include <stdio.h>
int main() 
{
    int n,i,count=0;
    printf("enter the value of n:");
    scanf("%d",&n);
    if(n==0||n==1)
     count=1;
    for(i=2;i<=n/2;i++)
    {
        if(n%i==0)
        {
            count = 1;
            break;
        }
    }
    if(count==0)
      printf("%d is a prime number",n);
    else
      printf("%d is not a prime number",n);
    return 0;
}
output:
enter the value of n:78
78 is not a prime number

6)write a c-program to check whether a given number is a pertect number or not
#include <stdio.h>
int main()
{
    int n,sum=0,i;
    printf("enter the valie of n:");
    scanf("%d",&n);
    for(i=1;i<=n/2 ;i++)
    { 
      if(n%i == 0)  
      {
          sum=sum+i;
      }
    }
    if(sum==n )
    {
        printf("%d is a perfect number",n);
    }
    else
    {
        printf("%d is not a perfect number",n);
    }
    return 0;
}
output:
1)enter the valie of n:6
6 is a perfect number
2)enter the valie of n:9
9 is not a perfect number

7)write a c-program that displays all the numbers from x and y,that are divisible by a and b.(x,y,a,b should be read from keyboard).

8)write a c-program to enter a decimal number and calculate and display the binary equivalent of that number

9)writa a c-program to find the roots of a quadratic equation
#include <stdio.h>
int main() {
    int num, originalNum, remainder, result = 0;
    printf("Enter a three-digit integer: ");
    scanf("%d", &num);
    originalNum = num;

    while (originalNum != 0) {
      
        remainder = originalNum % 10;
       result += remainder * remainder * remainder;
       originalNum /= 10;
    }

    if (result == num)
        printf("%d is an Armstrong number.", num);
    else
        printf("%d is not an Armstrong number.", num);

    return 0;
}
10)write c-program to whether the given number is armstrong number or not



















































