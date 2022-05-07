# (h1) 구현주의 일기장

## (h2) 목차
1. 자기소개
2. 오늘의 할 일
3. 코드

---

### (h3) 1. 자기소개
소프트웨어공학과 22학번 구현주

---

### (h3) 2. 오늘의 할일
* 깃 스터디 과제
* c언어 과제
* 영어회화 과제
* 일반물리실험 과제
* 수학 과제

---

### (h3) 3. 코드
##### (h5) 3-1. c언어 과제 문제1
~~~c
#include <stdio.h>
int main(){
	float r, result=1.0;
	int n, i;
	printf("실수의 값을 입력하시오. :");
	scanf("%f", &r);
	printf("거듭제곱의 값을 입력하시오. :");
	scanf("%d", &n);
	for(i=1; i<=n; i++){
		result*=r;
	}
	printf("결과값은 %f", result);
	return 0;
}
~~~
##### (h5) 3-1. c언어 과제 문제2
~~~c
#include <stdio.h>
int main(){
	int a=0, b=1, c, i, n; 
	printf("몇번째 항까지 구할까요? :");
	scanf("%d", &n);
	for(i=1; i<=n+1; i++){
		printf("%d, ", a);
		c=a+b;
		a=b;
		b=c;
	}
	return 0;
}
~~~

##### (h5) 3-1. c언어 과제 문제3
~~~c
#include <stdio.h>
int main(){
	int i=0, sum=0;
	while(1){
		i++;
		sum += i;
		if(sum>=10000){
			sum -= i;
			--i;
			break;
		}
	}
	printf("1부터 %d까지의 합이 %d입니다.", i, sum);
    return 0;
}
~~~
---