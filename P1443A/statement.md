## Description

<div><p>Today the kindergarten has a new group of $n$ kids who need to be seated at the dinner table. The chairs at the table are numbered from $1$ to $4n$. Two kids can't sit on the same chair. It is known that two kids who sit on chairs with numbers $a$ and $b$ ($a \neq b$) will indulge if: </p><ol> <li> $gcd(a, b) = 1$ or, </li><li> $a$ divides $b$ or $b$ divides $a$. </li></ol><p>$gcd(a, b)$&nbsp;— the maximum number $x$ such that $a$ is divisible by $x$ and $b$ is divisible by $x$.</p><p>For example, if $n=3$ and the kids sit on chairs with numbers $2$, $3$, $4$, then they will indulge since $4$ is divided by $2$ and $gcd(2, 3) = 1$. If kids sit on chairs with numbers $4$, $6$, $10$, then they will not indulge.</p><p>The teacher really doesn't want the mess at the table, so she wants to seat the kids so there are no $2$ of the kid that can indulge. More formally, she wants no pair of chairs $a$ and $b$ that the kids occupy to fulfill the condition above.</p><p>Since the teacher is very busy with the entertainment of the kids, she asked you to solve this problem.</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \leq t \leq 100$)&nbsp;— the number of test cases. Then $t$ test cases follow.</p><p>Each test case consists of one line containing an integer $n$ ($1 \leq n \leq 100$)&nbsp;— the number of kids.</p></div><div class="output-specification"><p>Output $t$ lines, which contain $n$ distinct integers from $1$ to $4n$&nbsp;— the numbers of chairs that the kids should occupy in the corresponding test case. If there are multiple answers, print any of them. You can print $n$ numbers in any order.</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \leq t \leq 100$)&nbsp;— the number of test cases. Then $t$ test cases follow.</p><p>Each test case consists of one line containing an integer $n$ ($1 \leq n \leq 100$)&nbsp;— the number of kids.</p>

## Output

<p>Output $t$ lines, which contain $n$ distinct integers from $1$ to $4n$&nbsp;— the numbers of chairs that the kids should occupy in the corresponding test case. If there are multiple answers, print any of them. You can print $n$ numbers in any order.</p>





```input1
3
2
3
4
```




```output1
6 4
4 6 10
14 10 12 8
```


