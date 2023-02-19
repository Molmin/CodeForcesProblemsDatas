## Description

<div><div class="epigraph"><div class="epigraph-text">The enchanted forest got its name from the magical mushrooms growing here. They may cause illusions and generally should not be approached.</div><div class="epigraph-source">—<span class="tex-font-style-it">Perfect Memento in Strict Sense</span></div></div><p>Marisa comes to pick mushrooms in the Enchanted Forest. </p><p>The Enchanted forest can be represented by $n$ points on the $X$-axis numbered $1$ through $n$. Before Marisa started, her friend, Patchouli, used magic to detect the initial number of mushroom on each point, represented by $a_1,a_2,\ldots,a_n$.</p><p>Marisa can start out at <span class="tex-font-style-bf">any</span> point in the forest on minute $0$. Each minute, the followings happen in order:</p><ul> <li> She moves from point $x$ to $y$ ($|x-y|\le 1$, possibly $y=x$). </li><li> She collects all mushrooms on point $y$. </li><li> A new mushroom appears on each point in the forest. </li></ul><p>Note that she <span class="tex-font-style-bf">cannot</span> collect mushrooms on minute $0$.</p><p>Now, Marisa wants to know the maximum number of mushrooms she can pick after $k$ minutes.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains a single integer $t$ ($1 \leq t \leq 10^4$) — the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains two integers $n$, $k$ ($1 \le n \le 2 \cdot 10 ^ 5$, $1\le k \le 10^9$) — the number of positions with mushrooms and the time Marisa has, respectively.</p><p>The second line of each test case contains $n$ integers $a_1,a_2,\ldots,a_n$ ($1 \le a_i \le 10^9$) — the initial number of mushrooms on point $1,2,\ldots,n$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10 ^ 5$.</p></div><div class="output-specification"><p>For each test case, print the maximum number of mushrooms Marisa can pick after $k$ minutes.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains a single integer $t$ ($1 \leq t \leq 10^4$) — the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains two integers $n$, $k$ ($1 \le n \le 2 \cdot 10 ^ 5$, $1\le k \le 10^9$) — the number of positions with mushrooms and the time Marisa has, respectively.</p><p>The second line of each test case contains $n$ integers $a_1,a_2,\ldots,a_n$ ($1 \le a_i \le 10^9$) — the initial number of mushrooms on point $1,2,\ldots,n$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10 ^ 5$.</p>

## Output

<p>For each test case, print the maximum number of mushrooms Marisa can pick after $k$ minutes.</p>





```input1|
4
5 2
5 6 1 2 3
5 7
5 6 1 2 3
1 2
999999
5 70000
1000000000 1000000000 1000000000 1000000000 1000000000
```




```output1
12
37
1000000
5000349985
```



## Note

<p>Test case 1:</p><p>Marisa can start at $x=2$. In the first minute, she moves to $x=1$ and collect $5$ mushrooms. The number of mushrooms will be $[1,7,2,3,4]$. In the second minute, she moves to $x=2$ and collects $7$ mushrooms. The numbers of mushrooms will be $[2,1,3,4,5]$. After $2$ minutes, Marisa collects $12$ mushrooms.</p><p>It can be shown that it is impossible to collect more than $12$ mushrooms.</p><p>Test case 2:</p><p>This is one of her possible moving path:</p><p>$2 \rightarrow 3 \rightarrow 2 \rightarrow 1 \rightarrow 2 \rightarrow 3 \rightarrow 4 \rightarrow 5$</p><p>It can be shown that it is impossible to collect more than $37$ mushrooms.</p>
