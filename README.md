//Programmers 1Level problem
// int num is even : return Even
// int num is odd : return Odd

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

