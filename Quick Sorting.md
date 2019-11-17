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
더듬이 처럼 벽에 붙히치지 않고 장애물을 구분하고 가는게 신기했고 다음에는 다른것을 좀더 연구해서 만들어보고싶습니다.
