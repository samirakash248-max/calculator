# calculator
This is my first git repo. I've given a basic calculator code in c language in this.
<br>
Author- Samir Akash
<br> 
<strong>The following is the c code for calculator , it can be run in any c compiler and used.</strong>
<br>

#include <stdio.h>

float add(float a,float b) {
    float sum=a+b;
    return sum;
}

float subtract(float a, float b){
    float sub=a-b;
    return sub;
}

float product(float a,float b){
    float pro=a*b;
    return pro;
}

float division(float a,float b){
    float div=a/b;
    return div;
}

int main() {
   printf("this is a calculator.\n Welcome!\n");
   float a;
   float b;
   int op;
   printf("enter the first number=");
   scanf("%f",&a);
   printf("Enter the second number=");
   scanf("%f",&b);
   printf("enter the operation you want to do(1=add,2=subtract,3=product,4=division)=");
   scanf("%d",&op);
   if (op==1){
       printf("the sum is=%.3f",add(a,b));
   }
   else if (op==2){
       printf("the subtacted value is=%.3f",subtract(a,b));
   }
   else if (op==3){
       printf("the product is=%.3f",product(a,b));
   }
   else if (op==4){
       printf("the division value is=%.3f",division(a,b));
   }
   else{
       printf("wrong input!Please select a valid operation!");
   }
   return 0;
}
