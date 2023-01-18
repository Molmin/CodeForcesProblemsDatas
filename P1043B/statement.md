## Description

<div><p>Bajtek, known for his unusual gifts, recently got an integer array $x_0, x_1, \ldots, x_{k-1}$.</p><p>Unfortunately, after a huge array-party with his extraordinary friends, he realized that he'd lost it. After hours spent on searching for a new toy, Bajtek found on the arrays producer's website another array $a$ of length $n + 1$. As a formal description of $a$ says, $a_0 = 0$ and for all other $i$&nbsp;($1 \le i \le n$) $a_i = x_{(i-1)\bmod k} + a_{i-1}$, where $p \bmod q$ denotes the remainder of division $p$ by $q$.</p><p>For example, if the $x = [1, 2, 3]$ and $n = 5$, then:</p><ul> <li> $a_0 = 0$, </li><li> $a_1 = x_{0\bmod 3}+a_0=x_0+0=1$, </li><li> $a_2 = x_{1\bmod 3}+a_1=x_1+1=3$, </li><li> $a_3 = x_{2\bmod 3}+a_2=x_2+3=6$, </li><li> $a_4 = x_{3\bmod 3}+a_3=x_0+6=7$, </li><li> $a_5 = x_{4\bmod 3}+a_4=x_1+7=9$. </li></ul><p>So, if the $x = [1, 2, 3]$ and $n = 5$, then $a = [0, 1, 3, 6, 7, 9]$.</p><p>Now the boy hopes that he will be able to restore $x$ from $a$! Knowing that $1 \le k \le n$, help him and find all possible values of $k$&nbsp;— possible lengths of the lost array.</p></div><div class="input-specification"><p>The first line contains exactly one integer $n$ ($1 \le n \le 1000$)&nbsp;— the length of the array $a$, excluding the element $a_0$.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 10^6$).</p><p>Note that $a_0$ is always $0$ and is not given in the input.</p></div><div class="output-specification"><p>The first line of the output should contain one integer $l$ denoting the number of correct lengths of the lost array.</p><p>The second line of the output should contain $l$ integers&nbsp;— possible lengths of the lost array in <span class="tex-font-style-bf">increasing</span> order.</p></div>

## Input

<p>The first line contains exactly one integer $n$ ($1 \le n \le 1000$)&nbsp;— the length of the array $a$, excluding the element $a_0$.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 10^6$).</p><p>Note that $a_0$ is always $0$ and is not given in the input.</p>

## Output

<p>The first line of the output should contain one integer $l$ denoting the number of correct lengths of the lost array.</p><p>The second line of the output should contain $l$ integers&nbsp;— possible lengths of the lost array in <span class="tex-font-style-bf">increasing</span> order.</p>





```input1
5
1 2 3 4 5

```




```input2
5
1 3 5 6 8

```




```input3
3
1 5 3

```




```output1
5
1 2 3 4 5
```




```output2
2
3 5
```




```output3
1
3
```



## Note

<p>In the first example, any $k$ is suitable, since $a$ is an arithmetic progression.</p><p>Possible arrays $x$:</p><ul> <li> $[1]$</li><li> $[1, 1]$</li><li> $[1, 1, 1]$</li><li> $[1, 1, 1, 1]$ </li><li> $[1, 1, 1, 1, 1]$</li></ul><p>In the second example, Bajtek's array can have three or five elements.</p><p>Possible arrays $x$:</p><ul> <li> $[1, 2, 2]$</li><li> $[1, 2, 2, 1, 2]$</li></ul><p>For example, $k = 4$ is bad, since it leads to $6 + x_0 = 8$ and $0 + x_0 = 1$, which is an obvious contradiction.</p><p>In the third example, only $k = n$ is good.</p><p>Array $[1, 4, -2]$ satisfies the requirements.</p><p>Note that $x_i$ may be negative.</p>
