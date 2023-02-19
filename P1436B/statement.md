## Description

<div><p>Sasha likes investigating different math objects, for example, magic squares. But Sasha understands that magic squares have already been studied by hundreds of people, so he sees no sense of studying them further. Instead, he invented his own type of square&nbsp;— a prime square. </p><p>A square of size $n \times n$ is called prime if the following three conditions are held simultaneously: </p><ul> <li> all numbers on the square are non-negative integers not exceeding $10^5$; </li><li> there are no prime numbers in the square; </li><li> sums of integers in each row and each column are prime numbers. </li></ul><p>Sasha has an integer $n$. He asks you to find any prime square of size $n \times n$. Sasha is absolutely sure such squares exist, so just help him!</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10$)&nbsp;— the number of test cases.</p><p>Each of the next $t$ lines contains a single integer $n$ ($2 \le n \le 100$)&nbsp;— the required size of a square.</p></div><div class="output-specification"><p>For each test case print $n$ lines, each containing $n$ integers&nbsp;— the prime square you built. If there are multiple answers, print any.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10$)&nbsp;— the number of test cases.</p><p>Each of the next $t$ lines contains a single integer $n$ ($2 \le n \le 100$)&nbsp;— the required size of a square.</p>

## Output

<p>For each test case print $n$ lines, each containing $n$ integers&nbsp;— the prime square you built. If there are multiple answers, print any.</p>





```input1
2
4
2
```




```output1
4 6 8 1
4 9 9 9
4 10 10 65
1 4 4 4
1 1
1 1
```


