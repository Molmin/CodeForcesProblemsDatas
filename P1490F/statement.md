## Description

<div><p>Polycarp was gifted an array $a$ of length $n$. Polycarp considers an array beautiful if there exists a number $C$, such that each number in the array occurs either zero or $C$ times. Polycarp wants to remove some elements from the array $a$ to make it beautiful.</p><p>For example, if $n=6$ and $a = [1, 3, 2, 1, 4, 2]$, then the following options are possible to make the array $a$ array beautiful: </p><ul> <li> Polycarp removes elements at positions $2$ and $5$, array $a$ becomes equal to $[1, 2, 1, 2]$; </li><li> Polycarp removes elements at positions $1$ and $6$, array $a$ becomes equal to $[3, 2, 1, 4]$; </li><li> Polycarp removes elements at positions $1, 2$ and $6$, array $a$ becomes equal to $[2, 1, 4]$; </li></ul><p>Help Polycarp determine the minimum number of elements to remove from the array $a$ to make it beautiful.</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases. Then $t$ test cases follow.</p><p>The first line of each test case consists of one integer $n$ ($1 \le n \le 2 \cdot 10^5$)&nbsp;— the length of the array $a$.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 10^9$)&nbsp;— array $a$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output one integer&nbsp;— the minimum number of elements that Polycarp has to remove from the array $a$ to make it beautiful.</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases. Then $t$ test cases follow.</p><p>The first line of each test case consists of one integer $n$ ($1 \le n \le 2 \cdot 10^5$)&nbsp;— the length of the array $a$.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 10^9$)&nbsp;— array $a$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, output one integer&nbsp;— the minimum number of elements that Polycarp has to remove from the array $a$ to make it beautiful.</p>





```input1
3
6
1 3 2 1 4 2
4
100 100 4 100
8
1 2 3 3 3 2 6 6
```




```output1
2
1
2
```


