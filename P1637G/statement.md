## Description

<div><p>Vitaly gave Maxim $n$ numbers $1, 2, \ldots, n$ for his $16$-th birthday. Maxim was tired of playing board games during the celebration, so he decided to play with these numbers. In one step Maxim can choose two numbers $x$ and $y$ from the numbers he has, throw them away, and add two numbers $x + y$ and $|x - y|$ instead. He wants all his numbers to be equal after several steps and the sum of the numbers to be minimal.</p><p>Help Maxim to find a solution. Maxim's friends don't want to wait long, so the number of steps in the solution should not exceed $20n$. It is guaranteed that under the given constraints, if a solution exists, then there exists a solution that makes all numbers equal, minimizes their sum, and spends no more than $20n$ moves.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 25\,000$)&nbsp;— the number of test cases.</p><p>Each test case contains a single integer $n$ ($2 \le n \le 5 \cdot 10^4$)&nbsp;— the number of integers given to Maxim.</p><p>It is guaranteed that the total sum of $n$ doesn't exceed $5 \cdot 10^4$.</p></div><div class="output-specification"><p>For each test case print $-1$ if it's impossible to make all numbers equal.</p><p>Otherwise print a single integer $s$ ($0 \le s \le 20n$)&nbsp;— the number of steps. Then print $s$ lines. The $i$-th line must contain two integers $x_i$ and $y_i$&nbsp;— numbers that Maxim chooses on the $i$-th step. The numbers must become equal after all operations.</p><p>Don't forget that you not only need to make all numbers equal, but also minimize their sum. It is guaranteed that under the given constraints, if a solution exists, then there exists a solution that makes all numbers equal, minimizes their sum, and spends no more than $20n$ moves.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 25\,000$)&nbsp;— the number of test cases.</p><p>Each test case contains a single integer $n$ ($2 \le n \le 5 \cdot 10^4$)&nbsp;— the number of integers given to Maxim.</p><p>It is guaranteed that the total sum of $n$ doesn't exceed $5 \cdot 10^4$.</p>

## Output

<p>For each test case print $-1$ if it's impossible to make all numbers equal.</p><p>Otherwise print a single integer $s$ ($0 \le s \le 20n$)&nbsp;— the number of steps. Then print $s$ lines. The $i$-th line must contain two integers $x_i$ and $y_i$&nbsp;— numbers that Maxim chooses on the $i$-th step. The numbers must become equal after all operations.</p><p>Don't forget that you not only need to make all numbers equal, but also minimize their sum. It is guaranteed that under the given constraints, if a solution exists, then there exists a solution that makes all numbers equal, minimizes their sum, and spends no more than $20n$ moves.</p>





```input1
2
2
3
```




```output1
-1
3
1 3
2 2
4 0
```


