## 1. Найти сложность приведенного ниже соотношения:  

$
T(n) = \begin{cases} 
    3T(n-1), &\text{если } n>0,\\
    1, &\text{иначе} 
\end{cases}
$
Решение: T(n) = 3T(n-1)= 3(3T(n-1-1)=3(3(3T-1-1-1)=3^nT(n-n)=3^nT(0)= 3^n
Ответ: 3^n

## 2. Найти сложность приведенного ниже соотношения:  
$
T(n) = \begin{cases} 
    2T(n-1) – 1 &\text{если } n>0,\\
    1, &\text{иначе} 
\end{cases}
$
Решение: T(n) = 2^n -(2^n-1) = 2^n-2^n +1 = 1
Ответ: О(1) 

## 3. Найти сложность приведенной ниже программы:

```python
def funct(n):
    if (n==1):
        return
    for i in range(1, n+1):
        for j in range(1, n + 1):
            print("*", end = "")
            break
          print()
```
Ответ: O(n) т.к если break, то выполняется 1 раз.

## 4. Найти сложность приведенной ниже программы:

```python
def funct(n):
    count = 0
    for i in range(n//2, n+1):
        j = 1                       n, while вложена
        while j <= n: 
            j = 2 * j  logn
            k = 1
            while k <= n:
                k = 2 * k  logn
                count += 1
```
Ответ: n*logn*logn =nlog^2n
## 5. Найти сложность приведенной ниже программы: 

```python
def funct(n):
    count = 0
    for i in range(n//2, n+1):    n
        j = 1
        while j + n // 2 <= n:   n, while вложена
            j += 1
            k = 1
            while k <= n:        logn, while вложена
                k = 2 * k
                count += 1
```
Ответ: n^2logn
## 6. Найти сложность приведенной ниже программы: 

```py
def function(n):
    i = 1
    s = 1
    while s <= n:
        i += 1
        s += i
        print('*')
```
Ответ: O(sqrt(n)
## 7. Найти сложность приведенной ниже программы: 

```py
def function(n):
    count = 0
    for i in range(n):            n 
        for j in range(i, i * i): n^2
            if j % i == 0:
                for k in range(j): n^2
                    print('*')
```
Ответ: O(n^5)
## 8. Найти сложность приведенной ниже программы: 

```python
def function(n):
    i = 1
    s = 1
    while (s < n):
        s = s + i
        i+=1
```

Ответ: O(sqrt(n)
## 9. Найти сложность приведенной ниже программы: 


```python
def fun(n):
    if (n < 5):
        print("Sirius", end ="")
    else:
        for i in range(n):
            print(i, end= " ")
```
Ответ: O(n)
## 10. Найти сложность приведенной ниже программы в лучшем и в худшем случае: 


```python
def fun(a, b):
    while (a != b):
        if (a > b):
            a = a - b
        else:
            b = b - a
```             
Ответ: в лучшем - O(1), в худшем - O(max{a/2, b/2})
## 11. Найти сложность приведенной ниже программы: 

```py
def fun(n):
    i = 0
    while i*i < n:
        print("Sirius")
        i += 1
```

Ответ: O(sqrt(n)
## 12. Найти сложность приведенной ниже программы: 

```py
def fun(n, x):
  for i in range(1, n, i * x):
    print("Sirius")
```
Ответ: logxn
## 13. Найти сложность приведенной ниже программы: 

```py
import math
 
def fun(n):
    for i in range(0,math.floor(n/2)):       n
        for j in range(1,n-math.floor(n/2)+1):  n
            k=1;
            for k in range(1,n+1,2*k):   n^2
                 print("Sirius");
```
Ответ: O(n^3)
## 14. Найти сложность приведенной ниже программы: 

```python
def fun(n):
    for i in range(1,n+1):
        for j in range(1,n+1,i):
            print("Sirius");

```

Ответ: O(sqrt(n)
## 15. Найти сложность приведенной ниже программы: 

```py
def fun(n):
    for i in range(n//3 + 1):
        for j in range(1, n+1, 4):
            print("Sirius")
```             

Ответ: O(sqrt(n)
## 16. Найти сложность приведенной ниже программы:  

```py
def fun(n):
    i = 1
    while (i < n):    logn
        j = n
        while (j > 0):
            j = j // 2  logn
        i = i * 2
```
Ответ: O(logn^2)
## 17. Найти какое число сравнений будет сделано при выполнении следующего фрагмента кода?  
```py
def fun(n):
    j = 1
    while (j <= n):
        j = j * 2     logn
```
Ответ: logn +1 
## 18. Найти сложность приведенной ниже программы: 
 
```py
a = 0
b = 0
for i in range(N):  O(n)
    a = a + random()
 
for i in range(M):  O(m), for не вложено
    b = b + random()
 ```
Ответ: O(n+m)
## 19. Найти сложность приведенной ниже программы: 
 
```py
a = 0;
for i in range(N):
    for j in reversed(range(i,N)):  n^2
        a = a + i + j;
 ```
Ответ: O(n^2)
## 20. Найти сложность приведенной ниже программы: 
 
```py
k = 0;
for i in range(n//2,n):  n 
    for j in range(2,n,pow(2,j)):  logn
        k = k + n / 2;
 `
Ответ: nlogn``

## 21. Найти сложность приведенной ниже программы: 
```py
a = 0
i = N
while (i > 0):
    a += i
    i //= 2
``` 
Ответ: O(logn)
## 22. Найти сложность приведенной ниже программы: 

```py
for i in range(n):
    i = i * k
```
Ответ: O(Logkn)
## 23. Найти сложность приведенной ниже программы: 

```py
value = 0
for i in range(n):
    for j in range(i):
        value = value + 1

Ответ: O(sqrt(n)
```
