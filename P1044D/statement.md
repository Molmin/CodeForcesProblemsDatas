## Description

<div><p>There is an array $a$ of $2^{30}$ integers, indexed from $0$ to $2^{30}-1$. Initially, you know that $0 \leq a_i &lt; 2^{30}$ ($0 \leq i &lt; 2^{30}$), but you do not know any of the values. Your task is to process queries of two types:</p><ul><li> <span class="tex-font-style-tt">1 l r x</span>: You are informed that the <span class="tex-font-style-bf">bitwise xor</span> of the subarray $[l, r]$ (ends inclusive) is equal to $x$. That is, $a_l \oplus a_{l+1} \oplus \ldots \oplus a_{r-1} \oplus a_r = x$, where $\oplus$ is the bitwise xor operator. In some cases, the received update contradicts past updates. In this case, you should <span class="tex-font-style-bf">ignore</span> the contradicting update (the current update).</li><li> <span class="tex-font-style-tt">2 l r</span>: You are asked to output the bitwise xor of the subarray $[l, r]$ (ends inclusive). If it is still impossible to know this value, considering all past updates, then output <span class="tex-font-style-tt">$-1$</span>.</li></ul><p>Note that the queries are <span class="tex-font-style-bf">encoded</span>. That is, you need to write an <span class="tex-font-style-bf">online</span> solution.</p></div><div class="input-specification"><p>The first line contains a single integer $q$ ($1 \leq q \leq 2 \cdot 10^5$)&nbsp;— the number of queries.</p><p>Each of the next $q$ lines describes a query. It contains one integer $t$ ($1 \leq t \leq 2$)&nbsp;— the type of query.</p><p>The given queries will be <span class="tex-font-style-bf">encoded</span> in the following way: let $last$ be the answer to the last query of the second type that you have answered (initially, $last = 0$). If the last answer was $-1$, set $last = 1$.</p><ul><li> If $t = 1$, three integers follow, $l'$, $r'$, and $x'$ ($0 \leq l', r', x' &lt; 2^{30}$), meaning that you got an update. <span class="tex-font-style-bf">First, do the following</span>:<center> $l = l' \oplus last$, $r = r' \oplus last$, $x = x' \oplus last$ </center><p>and, if $l &gt; r$, swap $l$ and $r$.</p><p>This means you got an update that the bitwise xor of the subarray $[l, r]$ is equal to $x$ (notice that you need to ignore updates that contradict previous updates).</p></li><li> If $t = 2$, two integers follow, $l'$ and $r'$ ($0 \leq l', r' &lt; 2^{30}$), meaning that you got a query. <span class="tex-font-style-bf">First, do the following</span>:<center> $l = l' \oplus last$, $r = r' \oplus last$ </center><p>and, if $l &gt; r$, swap $l$ and $r$.</p><p>For the given query, you need to print the bitwise xor of the subarray $[l, r]$. If it is impossible to know, print <span class="tex-font-style-tt">$-1$</span>. <span class="tex-font-style-bf">Don't forget to change the value of $last$</span>.</p></li></ul><p>It is guaranteed there will be at least one query of the second type.</p></div><div class="output-specification"><p>After every query of the second type, output the bitwise xor of the given subarray or <span class="tex-font-style-tt">$-1$</span> if it is still impossible to know.</p></div>

## Input

<p>The first line contains a single integer $q$ ($1 \leq q \leq 2 \cdot 10^5$)&nbsp;— the number of queries.</p><p>Each of the next $q$ lines describes a query. It contains one integer $t$ ($1 \leq t \leq 2$)&nbsp;— the type of query.</p><p>The given queries will be <span class="tex-font-style-bf">encoded</span> in the following way: let $last$ be the answer to the last query of the second type that you have answered (initially, $last = 0$). If the last answer was $-1$, set $last = 1$.</p><ul><li> If $t = 1$, three integers follow, $l'$, $r'$, and $x'$ ($0 \leq l', r', x' &lt; 2^{30}$), meaning that you got an update. <span class="tex-font-style-bf">First, do the following</span>:<center> $l = l' \oplus last$, $r = r' \oplus last$, $x = x' \oplus last$ </center><p>and, if $l &gt; r$, swap $l$ and $r$.</p><p>This means you got an update that the bitwise xor of the subarray $[l, r]$ is equal to $x$ (notice that you need to ignore updates that contradict previous updates).</p></li><li> If $t = 2$, two integers follow, $l'$ and $r'$ ($0 \leq l', r' &lt; 2^{30}$), meaning that you got a query. <span class="tex-font-style-bf">First, do the following</span>:<center> $l = l' \oplus last$, $r = r' \oplus last$ </center><p>and, if $l &gt; r$, swap $l$ and $r$.</p><p>For the given query, you need to print the bitwise xor of the subarray $[l, r]$. If it is impossible to know, print <span class="tex-font-style-tt">$-1$</span>. <span class="tex-font-style-bf">Don't forget to change the value of $last$</span>.</p></li></ul><p>It is guaranteed there will be at least one query of the second type.</p>

## Output

<p>After every query of the second type, output the bitwise xor of the given subarray or <span class="tex-font-style-tt">$-1$</span> if it is still impossible to know.</p>





```input1
12
2 1 2
2 1 1073741822
1 0 3 4
2 0 0
2 3 3
2 0 3
1 6 7 3
2 4 4
1 0 2 1
2 0 0
2 4 4
2 0 0

```




```input2
4
1 5 5 9
1 6 6 5
1 6 5 10
2 6 5

```




```output1
-1
-1
-1
-1
5
-1
6
3
5

```




```output2
12

```



## Note

<p>In the first example, the real queries (without being encoded) are:</p><ul><li> <span class="tex-font-style-tt">12</span></li><li> <span class="tex-font-style-tt">2 1 2</span></li><li> <span class="tex-font-style-tt">2 0 1073741823</span></li><li> <span class="tex-font-style-tt">1 1 2 5</span></li><li> <span class="tex-font-style-tt">2 1 1</span></li><li> <span class="tex-font-style-tt">2 2 2</span></li><li> <span class="tex-font-style-tt">2 1 2</span></li><li> <span class="tex-font-style-tt">1 2 3 6</span></li><li> <span class="tex-font-style-tt">2 1 1</span></li><li> <span class="tex-font-style-tt">1 1 3 0</span></li><li> <span class="tex-font-style-tt">2 1 1</span></li><li> <span class="tex-font-style-tt">2 2 2</span></li><li> <span class="tex-font-style-tt">2 3 3</span></li></ul><ul> <li> The answers for the first two queries are $-1$ because we don't have any such information on the array initially. </li><li> The first update tells us $a_1 \oplus a_2 = 5$. Note that we still can't be certain about the values $a_1$ or $a_2$ independently (for example, it could be that $a_1 = 1, a_2 = 4$, and also $a_1 = 3, a_2 = 6$). </li><li> After we receive all three updates, we have enough information to deduce $a_1, a_2, a_3$ independently. </li></ul><p>In the second example, notice that after the first two updates we already know that $a_5 \oplus a_6 = 12$, so the third update is contradicting, and we ignore it.</p>
