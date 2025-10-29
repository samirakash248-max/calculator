# calculator
This is my first git repo. I've given a basic calculator code in c language in this.
<br>
Author- Samir Akash
<br> 
<strong>The following is the c code for calculator , it can be run in any c compiler and used.</strong>
<br>

#include <stdio.h>

int add(int a,int b) {
    int sum;
    sum=a+b;
    return sum;
}

int subtract(int a, int b){
    int sub=a-b;
    return sub;
}

int product(int a,int b){
    int pro=a*b;
    return pro;
}

float division(float a,float b){
    float div=a/b;
    return div;
}

int main() {
   printf("this is a calculator.\n Welcome!\n");
   int a;
   int b;
   int op;
   printf("enter the first number=");
   scanf("%d",&a);
   printf("Enter the second number=");
   scanf("%d",&b);
   printf("enter the operation you want to do(1=add,2=subtract,3=product,4=division)=");
   scanf("%d",&op);
   if (op==1){
       printf("the sum is=%d",add(a,b));
   }
   else if (op==2){
       printf("the subtacted value is=%d",subtract(a,b));
   }
   else if (op==3){
       printf("the product is=%d",product(a,b));
   }
   else if (op==4){
       printf("the dision value is=%f",division(a,b));
   }
   else{
       printf("wrong input!");
   }
   return 0;
}
