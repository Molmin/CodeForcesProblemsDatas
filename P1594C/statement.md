## Description

<div><p>Theofanis has a string $s_1 s_2 \dots s_n$ and a character $c$. He wants to make all characters of the string equal to $c$ using the minimum number of operations.</p><p>In one operation he can choose a number $x$ ($1 \le x \le n$) and <span class="tex-font-style-bf">for every position $i$</span>, where $i$ is <span class="tex-font-style-bf">not</span> divisible by $x$, replace $s_i$ with $c$. </p><p>Find the minimum number of operations required to make all the characters equal to $c$ and the $x$-s that he should use in his operations.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains the integer $n$ ($3 \le n \le 3 \cdot 10^5$) and a lowercase Latin letter $c$&nbsp;— the length of the string $s$ and the character the resulting string should consist of.</p><p>The second line of each test case contains a string $s$ of lowercase Latin letters&nbsp;— the initial string.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $3 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, firstly print one integer $m$&nbsp;— the minimum number of operations required to make all the characters equal to $c$.</p><p>Next, print $m$ integers $x_1, x_2, \dots, x_m$ ($1 \le x_j \le n$)&nbsp;— the $x$-s that should be used in the order they are given.</p><p>It can be proved that under given constraints, an answer always exists. If there are multiple answers, print any.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains the integer $n$ ($3 \le n \le 3 \cdot 10^5$) and a lowercase Latin letter $c$&nbsp;— the length of the string $s$ and the character the resulting string should consist of.</p><p>The second line of each test case contains a string $s$ of lowercase Latin letters&nbsp;— the initial string.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $3 \cdot 10^5$.</p>

## Output

<p>For each test case, firstly print one integer $m$&nbsp;— the minimum number of operations required to make all the characters equal to $c$.</p><p>Next, print $m$ integers $x_1, x_2, \dots, x_m$ ($1 \le x_j \le n$)&nbsp;— the $x$-s that should be used in the order they are given.</p><p>It can be proved that under given constraints, an answer always exists. If there are multiple answers, print any.</p>





```input1
3
4 a
aaaa
4 a
baaa
4 b
bzyx
```




```output1
0
1
2
2 
2 3
```



## Note

<p>Let's describe what happens in the third test case: </p><ol> <li> $x_1 = 2$: we choose all positions that are not divisible by $2$ and replace them, i.&nbsp;e. <span class="tex-font-style-tt"><span class="tex-font-style-underline">b</span>z<span class="tex-font-style-underline">y</span>x</span> $\rightarrow$ <span class="tex-font-style-tt">bzbx</span>; </li><li> $x_2 = 3$: we choose all positions that are not divisible by $3$ and replace them, i.&nbsp;e. <span class="tex-font-style-tt"><span class="tex-font-style-underline">bz</span>b<span class="tex-font-style-underline">x</span></span> $\rightarrow$ <span class="tex-font-style-tt">bbbb</span>. </li></ol>
