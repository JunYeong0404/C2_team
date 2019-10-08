# C2_team
1.
##  1) test.c
#include<stdio.h>  
int add(int a, int b);  
int sub(int a, int b);  
int mul(int a, int b);  
int div(int a, int b);  
int modula(int a, int b);  
double result(float a, float b);  
int main(){  
int a=3, b=2;  
printf("%d\n", add(a,b));  
printf("%d\n", sub(a,b));  
printf("%d\n", mul(a,b));  
printf("%d\n", div(a,b));  
printf("%d\n", modula(a,b));  
printf("%.1f\n", result(a,b));  
}  

## 2)add.c
int add(int a, int b){  
return(a+b);  
}  

## 3)sub.c
int sub(int a, int b){  
return(a-b);  
}  

## 4)mul.c
int mul(int a, int b){  
return(a*b);  
}  

## 5)div.c
int div(int a, int b){  
return(a/b);  
}  
## 6)modula.c
int modula(int a, int b){  
return(a%b);  
}  
## 7)result.c
double result(float a, float b){  
return(a/b);  
}  

## 코멘트
 먼저 main폴더를 test폴더로 바꾼 후 add, sub, mul, div, modula, result 파일을 만든 후 소스 코드를 기계어로 바꿔서 나머지는 교수님이 알려주신데로 했습니다. 소수점은 int가 float를 받지 못해서 double로 바꿔서 했습니다.
 
 ## 소감
 교수님 오늘 수업은 엄청 어려웠지만 교수님이 알려주신걸 노트에 필기하고 소수점 나타내는걸 몰랐는데 친구들한테 물어보고 알아서 매우 뿌듯했습니다. 교수님이 너무 잘 가르쳐 주신거 같아서 성공할 수 있었던거 같습니다. 감사합니다. C언어 사랑합니다.
 
