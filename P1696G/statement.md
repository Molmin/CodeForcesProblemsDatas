## Description

<div><p>Suppose you are given a 1-indexed sequence $a$ of non-negative integers, whose length is $n$, and two integers $x$, $y$. In consecutive $t$ seconds ($t$ can be any positive real number), you can do one of the following operations:</p><ul> <li> Select $1\le i&lt;n$, decrease $a_i$ by $x\cdot t$, and decrease $a_{i+1}$ by $y\cdot t$. </li><li> Select $1\le i&lt;n$, decrease $a_i$ by $y\cdot t$, and decrease $a_{i+1}$ by $x\cdot t$. </li></ul><p>Define the minimum amount of time (it might be a real number) required to make all elements in the sequence less than or equal to $0$ as $f(a)$.</p><p>For example, when $x=1$, $y=2$, it takes $3$ seconds to deal with the array $[3,1,1,3]$. We can:</p><ul> <li> In the first $1.5$ seconds do the second operation with $i=1$. </li><li> In the next $1.5$ seconds do the first operation with $i=3$. </li></ul><p>We can prove that it's not possible to make all elements less than or equal to $0$ in less than $3$ seconds, so $f([3,1,1,3])=3$.</p><p>Now you are given a 1-indexed sequence $b$ of positive integers, whose length is $n$. You are also given positive integers $x$, $y$. Process $q$ queries of the following two types:</p><ul> <li> <span class="tex-font-style-tt">1 k v</span>: change $b_k$ to $v$. </li><li> <span class="tex-font-style-tt">2 l r</span>: print $f([b_l,b_{l+1},\dots,b_r])$. </li></ul></div><div class="input-specification"><p>The first line of input contains two integers $n$ and $q$ ($2\le n\le 2\cdot 10^5$, $1\le q\le 2\cdot 10^5$).</p><p>The second line of input contains two integers $x$ and $y$ ($1\le x,y\le 10^6$).</p><p>The third line of input contains $n$ integers $b_1,b_2,\ldots,b_n$ ($1\le b_i\le 10^6$).</p><p>This is followed by $q$ lines. Each of these $q$ lines contains three integers. The first integer $op$ is either $1$ or $2$.</p><ul> <li> If it is $1$, it is followed by two integers $k$, $v$ ($1\le k\le n$, $1\le v\le 10^6$). It means that you should change $b_k$ to $v$. </li><li> If it is $2$, it is followed by two integers $l$, $r$ ($1\le l&lt;r\le n$). It means that you should print $f([b_l,b_{l+1},\dots,b_r])$. </li></ul></div><div class="output-specification"><p>For each query of type $2$, print one real number — the answer to the query. Your answer is considered correct if its absolute error or relative error does not exceed $10^{-9}$.</p></div>

## Input

<p>The first line of input contains two integers $n$ and $q$ ($2\le n\le 2\cdot 10^5$, $1\le q\le 2\cdot 10^5$).</p><p>The second line of input contains two integers $x$ and $y$ ($1\le x,y\le 10^6$).</p><p>The third line of input contains $n$ integers $b_1,b_2,\ldots,b_n$ ($1\le b_i\le 10^6$).</p><p>This is followed by $q$ lines. Each of these $q$ lines contains three integers. The first integer $op$ is either $1$ or $2$.</p><ul> <li> If it is $1$, it is followed by two integers $k$, $v$ ($1\le k\le n$, $1\le v\le 10^6$). It means that you should change $b_k$ to $v$. </li><li> If it is $2$, it is followed by two integers $l$, $r$ ($1\le l&lt;r\le n$). It means that you should print $f([b_l,b_{l+1},\dots,b_r])$. </li></ul>

## Output

<p>For each query of type $2$, print one real number — the answer to the query. Your answer is considered correct if its absolute error or relative error does not exceed $10^{-9}$.</p>





```input1
4 3
1 2
3 1 1 4
2 1 4
1 1 1
2 1 3
```




```output1
3.500000000000000
1.000000000000000
```



## Note

<p>Let's analyse the sample.</p><p>In the first query, we are asked to compute $f([3,1,1,4])$. The answer is $3.5$. One optimal sequence of operations is:</p><ul> <li> In the first $1.5$ seconds do the second operation with $i=1$. </li><li> In the next $2$ seconds do the first operation with $i=3$. </li></ul><p>In the third query, we are asked to compute $f([1,1,1])$. The answer is $1$. One optimal sequence of operations is:</p><ul> <li> In the first $0.5$ seconds do the second operation with $i=1$. </li><li> In the next $0.5$ seconds do the first operation with $i=2$. </li></ul>
