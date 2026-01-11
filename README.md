# Lab_13_dz
Домашняя работа к лабораторной работе №13

# Условия задачи
Печать первой буквы каждого слова

# Блоксхема
<img width="472" height="1032" alt="flowchart_1768168975526" src="https://github.com/user-attachments/assets/a0903d96-921d-4587-899e-6266e5407589" />

# Реализация программы
```
#define _CRT_SECURE_NO_DEPRECATE
#include<stdio.h>
#include<locale.h>
#include<string.h>


char slovo[1000];
int c = 0;

int main() {

	setlocale(LC_ALL, "RUS");
	puts("Введите строку");
    fgets(slovo, sizeof(slovo), stdin);
    printf("%c", slovo[0]);
    for (int i = 1; i < strlen(slovo) - 1; i++) {
        if (slovo[i - 1] == ' ') {

            printf("%c", slovo[i]);
        }
    }

	return 0;
}
```
<img width="939" height="253" alt="image" src="https://github.com/user-attachments/assets/f5937ae4-30c8-45a3-b35a-cb01e3447db5" />
