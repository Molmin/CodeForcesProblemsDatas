## Description

<div><p>You are given an integer $n$.</p><p>Your task is to find two positive (greater than $0$) integers $a$ and $b$ such that $a+b=n$ and the least common multiple (LCM) of $a$ and $b$ is the minimum among all possible values of $a$ and $b$. If there are multiple answers, you can print any of them.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 100$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($2 \le n \le 10^9$).</p></div><div class="output-specification"><p>For each test case, print two positive integers $a$ and $b$&nbsp;— the answer to the problem. If there are multiple answers, you can print any of them.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 100$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($2 \le n \le 10^9$).</p>

## Output

<p>For each test case, print two positive integers $a$ and $b$&nbsp;— the answer to the problem. If there are multiple answers, you can print any of them.</p>





```input1|2,4
4
2
9
5
10
```




```output1
1 1
3 6
1 4
5 5
```



## Note

<p>In the second example, there are $8$ possible pairs of $a$ and $b$:</p><ul> <li> $a = 1$, $b = 8$, $LCM(1, 8) = 8$; </li><li> $a = 2$, $b = 7$, $LCM(2, 7) = 14$; </li><li> $a = 3$, $b = 6$, $LCM(3, 6) = 6$; </li><li> $a = 4$, $b = 5$, $LCM(4, 5) = 20$; </li><li> $a = 5$, $b = 4$, $LCM(5, 4) = 20$; </li><li> $a = 6$, $b = 3$, $LCM(6, 3) = 6$; </li><li> $a = 7$, $b = 2$, $LCM(7, 2) = 14$; </li><li> $a = 8$, $b = 1$, $LCM(8, 1) = 8$. </li></ul><p>In the third example, there are $5$ possible pairs of $a$ and $b$:</p><ul> <li> $a = 1$, $b = 4$, $LCM(1, 4) = 4$; </li><li> $a = 2$, $b = 3$, $LCM(2, 3) = 6$; </li><li> $a = 3$, $b = 2$, $LCM(3, 2) = 6$; </li><li> $a = 4$, $b = 1$, $LCM(4, 1) = 4$. </li></ul>
