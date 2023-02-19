## Description

<div><p>There are $n$ fishermen who have just returned from a fishing trip. The $i$-th fisherman has caught a fish of size $a_i$.</p><p>The fishermen will choose some order in which they are going to tell the size of the fish they caught (the order is just a permutation of size $n$). However, they are not entirely honest, and they may "increase" the size of the fish they have caught.</p><p>Formally, suppose the chosen order of the fishermen is $[p_1, p_2, p_3, \dots, p_n]$. Let $b_i$ be the value which the $i$-th fisherman in the order will tell to the other fishermen. The values $b_i$ are chosen as follows:</p><ul> <li> the first fisherman in the order just honestly tells the actual size of the fish he has caught, so $b_1 = a_{p_1}$; </li><li> every other fisherman wants to tell a value that is <span class="tex-font-style-bf">strictly greater</span> than the value told by the previous fisherman, and is divisible by the size of the fish that the fisherman has caught. So, for $i &gt; 1$, $b_i$ is the smallest integer that is both <span class="tex-font-style-bf">strictly greater</span> than $b_{i-1}$ and <span class="tex-font-style-bf">divisible by</span> $a_{p_i}$. </li></ul><p>For example, let $n = 7$, $a = [1, 8, 2, 3, 2, 2, 3]$. If the chosen order is $p = [1, 6, 7, 5, 3, 2, 4]$, then:</p><ul> <li> $b_1 = a_{p_1} = 1$; </li><li> $b_2$ is the smallest integer divisible by $2$ and greater than $1$, which is $2$; </li><li> $b_3$ is the smallest integer divisible by $3$ and greater than $2$, which is $3$; </li><li> $b_4$ is the smallest integer divisible by $2$ and greater than $3$, which is $4$; </li><li> $b_5$ is the smallest integer divisible by $2$ and greater than $4$, which is $6$; </li><li> $b_6$ is the smallest integer divisible by $8$ and greater than $6$, which is $8$; </li><li> $b_7$ is the smallest integer divisible by $3$ and greater than $8$, which is $9$. </li></ul><p>You have to choose the order of fishermen in a way that yields the minimum possible $\sum\limits_{i=1}^{n} b_i$.</p></div><div class="input-specification"><p>The first line contains one integer $n$ ($1 \le n \le 1000$) — the number of fishermen.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^6$).</p></div><div class="output-specification"><p>Print one integer — the minimum possible value of $\sum\limits_{i=1}^{n} b_i$ you can obtain by choosing the order of fishermen optimally.</p></div>

## Input

<p>The first line contains one integer $n$ ($1 \le n \le 1000$) — the number of fishermen.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^6$).</p>

## Output

<p>Print one integer — the minimum possible value of $\sum\limits_{i=1}^{n} b_i$ you can obtain by choosing the order of fishermen optimally.</p>





```input1
7
1 8 2 3 2 2 3
```




```input2
10
5 6 5 6 5 6 5 6 5 6
```




```output1
33
```




```output2
165
```


