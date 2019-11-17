퀵쇼팅 코드
***********

 #include<stdio.h>
 
 #define LEN 8

 void qs(int v[],int left,int right){
 
  int pivot,pi,l,r, dir;
  
 if(left<right){
 
  dir = 0;
  
  l=left; r=right; pi=left; 
  
  pivot = v[pi];
  
  while(l<r){
  
   if(dir==0){
   
  if(pivot<v[r] ) r--;
    
  else{
    
  v[pi]=v[r];
     
  pi = r;
    
 if(l!=r) l++;
     
 dir=1;
     
  }
    
  }
   
  if(dir==1){
   
  if(pivot>v[l]) l++;
    
  else{
    
  v[pi]=v[l];
      pi = l;
     
if(l!=r) r--;
     
 dir=0;
     
 }  
     }
  
 }
  
v[r] = pivot;
  
qs(v,left,r-1);
  
qs(v,r+1,right);
  
}
 
return;
 
 
}

void main(){

int i;
 
int v[LEN]={8,17,6,5,-44,3,2,1};
 
for(i=0;i<LEN;i++) printf(" %d", v[i]); printf("\n");
 
qs(v,0,LEN-1);

for(i=0;i<LEN;i++) printf(" %d", v[i]); printf("\n");
 
}

**소감**
********
버블쇼팅이랑 비슷한줄 알았지만 조금 다른것같아 어려운 느낌이 있었지만 유튜브 영상을 참고하여 보니 이해되는것같았습니다.
