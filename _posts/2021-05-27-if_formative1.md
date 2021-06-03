---
layout: single
title: ""
toc: true
toc_sticky: true
toc_label: "페이지 주요 목차"

categories: "형성평가"
---

### 01. 사주보기
![saju](/images/saju.jpg)

~~~c

#include <stdio.h>
 
int main(void) {
 int year, month, day, res;
 printf("당신의 사주를 봐드립니다. \n연도 월 일을 차례대로 입력하세요 : ");
 scanf("%d %d %d", &year, &month, &day);
 res=year-month+day;
  if((res%10)==0){
   printf("당신의 사주는 대박입니다.");
 }
 else {
   printf("당신의 사주는 그럭저럭입니다.");
 } 


### 02. 3개의 터널 통과
![tunnel](/images/tunnel.jpg)

~~~c

#include <stdio.h>
 
int main(void) {
 int a,b,c;
 
 printf("세 터널의 높이를 차례대로 입력하세요 : ");
 scanf("%d %d %d",&a,&b,&c);
 
 if(a<=170){
   printf("충돌 %d",a);
 }
  else if(b<=170){
 printf("충돌 %d",b); 
 }
 
 else if(c<=170){
 printf("충돌 %d",c);
 }
 
 else{
 printf("무사 통과");
 }
 
}


### 03. 이 달은 며칠까지 있을까?
![callender](/images/callender.jpg)

~~~c
#include <stdio.h>
 
int main(void) {
int year, month;
printf("연도와 월을 입력하세요 : ");
scanf("%d %d", &year, &month);
printf("%d년 %d월의 마지막 날은 ", year, month);
if(month==1 || month==3 || month==5 || month==7 || month==8 || month==10 || month==12){
printf("31일");
}
else if(month==4 || month==6 || month==9 || month==11){
printf("30일");
}
 
else
{
 if((year%4==0 && !(year%100==0)) || year%400==0)
 printf("29일");
 
 else
 printf("28일");
}
 
printf("입니다");
 
}

### 04. 30분 전은 몇 시 몇 분일까? 
![30minutes](/images/30minutes.jpg)

~~~c
#include <stdio.h>
 
int main(void) {
 int hour, min;
 printf("시간과 분을 입력하세요 : ");
 scanf("%d %d", &hour,&min);
 printf("입력한 시간의 30분 전 시간은 ");
 if(min>=30){
       printf("%d시 %d분", hour, min-30);
 }
 else{
   if(hour>0){
    printf("%d시 %d분", hour-1, min+30);
   }
  
   else{
    printf("%d시 %d분", hour+23, min+30);
   }
 }
 
}

### 05. 도어락 문제
![doorlock](/images/doorlock.png)

~~~c
#include <stdio.h>
 
int main(void) {
 char card;
 int key, choose;
 double gimun;
 
printf(">>장치 선택: ");
 scanf("%d", &choose);
 
if(choose==1){
 
 printf("IC 카드: ");
 scanf(" %c", &card);
 
 if(card=='c'){
   printf("문 열림~");
 }
 
 else {
   printf("디리릭!디리릭!");
 }
}
 
else if(choose==2){
 
printf("비밀번호: ");
 scanf("%d", &key);
 
 if(key==24680){
   printf("문 열림~");
 }
 
 else {
   printf("디리릭!디리릭!");
 }
}
 
else{
 
printf("지문 입력: ");
 scanf("%lf", &gimun);
 
 if(gimun==1.2345678){
   printf("문 열림~");
 }
 
 else {
   printf("디리릭!디리릭!");
 }
}
 return 0;
}

### 06. 가위바위보
![rockscissorpaper](/images/rockscissorpaper.png)

~~~c
#include <stdio.h>

int main(void) {
  
  char rsp, com;
  com = 's';
  printf("사용자 입력(가위:s, 바위:r, 보:p): ");
  scanf( "%c", &rsp);
 

  if(rsp == com){
  printf("비겼다");
  }

  else if((rsp =='r' && com == 's') || (rsp =='p' && com == 'r') || (rsp =='s' && com == 'p')){
  printf("이겼다");
  }

  else{
  printf("졌다");  
  }
  return 0;
}

### 07. 용돈으로 책 구입하기
![용돈으로 책 구입하기](images/용돈으로 책 구입하기.jpg)

~~~c
#include <stdio.h>

int main(void) {
  int hour, min;
  printf("시간과 분을 입력하세요 : ");
  scanf("%d %d", &hour,&min);
  printf("입력한 시간의 30분 전 시간은 ");
  if(min>=30){
        printf("%d시 %d분", hour, min-30);
  }
  else{
    if(hour>0){
     printf("%d시 %d분", hour-1, min+30);
    }
    
    else{
     printf("%d시 %d분", hour+23, min+30);
    }
  }
  

}
