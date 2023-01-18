## Description

<div><p>Toad Ivan has $m$ pairs of integers, each integer is between $1$ and $n$, inclusive. The pairs are $(a_1, b_1), (a_2, b_2), \ldots, (a_m, b_m)$. </p><p>He asks you to check if there exist two integers $x$ and $y$ ($1 \leq x &lt; y \leq n$) such that in each given pair at least one integer is equal to $x$ or $y$.</p></div><div class="input-specification"><p>The first line contains two space-separated integers $n$ and $m$ ($2 \leq n \leq 300\,000$, $1 \leq m \leq 300\,000$)&nbsp;— the upper bound on the values of integers in the pairs, and the number of given pairs.</p><p>The next $m$ lines contain two integers each, the $i$-th of them contains two space-separated integers $a_i$ and $b_i$ ($1 \leq a_i, b_i \leq n, a_i \neq b_i$)&nbsp;— the integers in the $i$-th pair.</p></div><div class="output-specification"><p>Output "<span class="tex-font-style-tt">YES</span>" if there exist two integers $x$ and $y$ ($1 \leq x &lt; y \leq n$) such that in each given pair at least one integer is equal to $x$ or $y$. Otherwise, print "<span class="tex-font-style-tt">NO</span>". You can print each letter in any case (upper or lower).</p></div>

## Input

<p>The first line contains two space-separated integers $n$ and $m$ ($2 \leq n \leq 300\,000$, $1 \leq m \leq 300\,000$)&nbsp;— the upper bound on the values of integers in the pairs, and the number of given pairs.</p><p>The next $m$ lines contain two integers each, the $i$-th of them contains two space-separated integers $a_i$ and $b_i$ ($1 \leq a_i, b_i \leq n, a_i \neq b_i$)&nbsp;— the integers in the $i$-th pair.</p>

## Output

<p>Output "<span class="tex-font-style-tt">YES</span>" if there exist two integers $x$ and $y$ ($1 \leq x &lt; y \leq n$) such that in each given pair at least one integer is equal to $x$ or $y$. Otherwise, print "<span class="tex-font-style-tt">NO</span>". You can print each letter in any case (upper or lower).</p>





```input1
4 6
1 2
1 3
1 4
2 3
2 4
3 4
```




```input2
5 4
1 2
2 3
3 4
4 5
```




```input3
300000 5
1 2
1 2
1 2
1 2
1 2
```




```output1
NO
```




```output2
YES
```




```output3
YES
```



## Note

<p>In the first example, you can't choose any $x$, $y$ because for each such pair you can find a given pair where both numbers are different from chosen integers.</p><p>In the second example, you can choose $x=2$ and $y=4$.</p><p>In the third example, you can choose $x=1$ and $y=2$.</p>
