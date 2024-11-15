#include<stdio.h>
int main(){
int a,b,x1,X2;
long long c;
printf("donne a:");
scanf("%d",&a);
printf("donne b:");
scanf("%d",&b);
int p = 10;
int s = 1;
do{
    x1 = a % 10;
    X2 = b % 10;
    c = x1 * p + X2 * s;
    p *= 10;
    s *= 10;
    a = a / 10;
    //a = a % 10;
    b = b / 10;
   // b = b % 10;
}while (a ==! 0 && b ==!0);
printf("c= %lld",c);
    return 0;
}
