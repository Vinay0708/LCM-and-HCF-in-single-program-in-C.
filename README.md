# LCM-and-HCF-in-single-program-in-C.
/*LCM of two numbers is HCF(a,b)*LCM(a,b)=a*b */
/* since LCM of two number is= (a*b)/HCF(a*b) */


#include <stdio.h>
int main()
{   int i,a,b,min,abtakkahcf,LCM;
   printf("Enter two numbers for checking HCF and LCM:\n");
   scanf("%d %d",&a,&b);
   min=a<b?a:b;
    for(i=1;i<=min;i++)
   {
       if(a%i==0 && b%i==0)
       abtakkahcf=i;
   }
   LCM=(a*b)/abtakkahcf;
   printf("The HCF OF %d and %d is %d\n",a,b,abtakkahcf);
   printf("the LCM OF %d and %d is %d",a,b,LCM);
    return 0;
}
