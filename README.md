/*Programmers 1Level problem
int num is even : return Even
int num is odd : return Odd
문제 설명
정수 num이 짝수일 경우 "Even"을 반환하고 홀수인 경우 "Odd"를 반환하는 함수, solution을 완성해주세요.

제한 조건
num은 int 범위의 정수입니다.
0은 짝수입니다.
https://programmers.co.kr/learn/courses/30/lessons/12937
*/

#include <stdio.h>
#include <stdbool.h>
#include <stdlib.h>

char* solution(int num) {
	char* answer = (char*)malloc(sizeof(char));
	if (num % 2 == 0)
		answer = "Even";
	else
		answer = "Odd";
	return answer;
}

int main(void)
{
	int num;
	char* ans;
	printf("숫자를 입력하시오 : ");
	scanf_s("%d", &num);
	ans = solution(num);
	printf("answer = %s \n", ans);
	
}

