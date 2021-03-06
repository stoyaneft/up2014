Домашно 3
=========

*Soft deadline (препоръчителен срок за предаване): до 15.01 23:59:59*

**Hard deadline (краен срок за предаване): до началото на сесията

### Задача 1 (10 точки) ###

Да се дефинира булева функция ```checkDivisors```, която проверява дали числото има подадения брой делители.

#### Сигнатура ####

```C++
bool checkDivisors(int number, int divisorsCount);
```

### Примери ###

```C++
checkDivisors(6, 4); // -> true
checkDivisors(12, 6); // -> true
checkDivisors(17, 3); // -> false
```

### Задача 2 (10 точки) ###

Да се дефинира функцията ```isMember```, която по дадени цяло число и масив от
цели числа казва дали числото се съдържа в масива.

#### Сигнатура ####

```C++
bool isMember(int number, int arr[], int n);
```

#### Примери ####

```C++
int arr[] = {1, 2, 3, 4, 5};
isMember(0, arr, 5); // -> false

int arr[] = {34, 934, 7, 0, 3, -1, 3};
isMember(3, arr, 7); // -> true

int arr[] = {1};
isMember(-1, arr, 1); // -> false
```

### Задача 3 (20 точки) ###

Щастливо число е число, изведено по следния начин: започвайки от произволно положително число,
замести числото със сумата от квадратите на всяка цифра в него, и продължи процеса, докато полученият резултат е равен
на 1 (където ще се задържи), или безкрайно ще се върти в цикъл, който не съдържа 1. Числата, които стигат до 1 са щастливи,
останалите - не.

Например, 19 е щастливо число, защото:

1^2 + 9^2 = 82

8^2 + 2^2 = 68

6^2 + 8^2 = 100

1^2 + 0^2 + 0^2 = 1

Да се дефинира булева функция ```isHappy```, която проверява дали едно число е щастливо. 

### Сигнатура ###
```C++
bool isHappy(int number);
```

### Примери ###

```C++
isHappy(10); // -> True
isHappy(11); // -> False
isHappy(7); // -> True
isHappy(512); // False
```
### Задача 4 (15 точки) ###

Да се дефинира функция ```happyPrimes```, която приема масив от цели числа и масив, в който записва всички числа, които са едновременно прости и щастливи. За целта да се ползва функцията от задача 3. Като последно число във втория масив сложете числото -1, което ще отбелязва, че няма повече такива числа.

### Сигнатура ###
```C++
void happyPrimes(int n, int* arr, int* happyPrimes);
```

### Примери ###

```C++
int arr[] = {1, 2, 3, ..., 24, 25};
int happyPrimes[26];
happyPrimes(25, arr, happyPrimes); // happyPrimes = {7, 13, 19, 23} 
int arr[] = {63, 64, ..., 99, 100};
int happyPrimes[39];
happyPrimes(25, arr, happyPrimes); // happyPrimes = {79, 97}
```
