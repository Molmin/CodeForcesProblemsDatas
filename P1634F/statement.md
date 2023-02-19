## Description

<div><div class="epigraph"><div class="epigraph-text">One of my most productive days was throwing away 1,000 lines of code.</div><div class="epigraph-source">— Ken Thompson</div></div><p><span class="tex-font-style-bf">Fibonacci addition</span> is an operation on an array $X$ of integers, parametrized by indices $l$ and $r$. Fibonacci addition increases $X_l$ by $F_1$, increases $X_{l + 1}$ by $F_2$, and so on up to $X_r$ which is increased by $F_{r - l + 1}$.</p><p>$F_i$ denotes the $i$-th Fibonacci number ($F_1 = 1$, $F_2 = 1$, $F_{i} = F_{i - 1} + F_{i - 2}$ for $i &gt; 2$), and <span class="tex-font-style-bf">all operations are performed modulo $MOD$</span>.</p><p>You are given two arrays $A$ and $B$ of the same length. We will ask you to perform several Fibonacci additions on these arrays with different parameters, and after each operation you have to report whether arrays $A$ and $B$ are equal modulo $MOD$.</p></div><div class="input-specification"><p>The first line contains 3 numbers $n$, $q$ and $MOD$ ($1 \le n, q \le 3\cdot 10^5, 1 \le MOD \le 10^9+7$)&nbsp;— the length of the arrays, the number of operations, and the number modulo which all operations are performed.</p><p>The second line contains $n$ numbers&nbsp;— array $A$ ($0 \le A_i &lt; MOD$).</p><p>The third line also contains $n$ numbers&nbsp;— array $B$ ($0 \le B_i &lt; MOD$).</p><p>The next $q$ lines contain character $c$ and two numbers $l$ and $r$ ($1 \le l \le r \le n$)&nbsp;— operation parameters. If $c$ is "A", Fibonacci addition is to be performed on array $A$, and if it is is "B", the operation is to be performed on $B$.</p></div><div class="output-specification"><p>After each operation, print "YES" (without quotes) if the arrays are equal and "NO" otherwise. Letter case does not matter.</p></div>

## Input

<p>The first line contains 3 numbers $n$, $q$ and $MOD$ ($1 \le n, q \le 3\cdot 10^5, 1 \le MOD \le 10^9+7$)&nbsp;— the length of the arrays, the number of operations, and the number modulo which all operations are performed.</p><p>The second line contains $n$ numbers&nbsp;— array $A$ ($0 \le A_i &lt; MOD$).</p><p>The third line also contains $n$ numbers&nbsp;— array $B$ ($0 \le B_i &lt; MOD$).</p><p>The next $q$ lines contain character $c$ and two numbers $l$ and $r$ ($1 \le l \le r \le n$)&nbsp;— operation parameters. If $c$ is "A", Fibonacci addition is to be performed on array $A$, and if it is is "B", the operation is to be performed on $B$.</p>

## Output

<p>After each operation, print "YES" (without quotes) if the arrays are equal and "NO" otherwise. Letter case does not matter.</p>





```input1
3 5 3
2 2 1
0 0 0
A 1 3
A 1 3
B 1 1
B 2 2
A 3 3
```




```input2
5 3 10
2 5 0 3 5
3 5 8 2 5
B 2 3
B 3 4
A 1 2
```




```output1
YES
NO
NO
NO
YES
```




```output2
NO
NO
YES
```



## Note

<p>Explanation of the test from the condition:</p><ul><li> Initially $A=[2,2,1]$, $B=[0,0,0]$.</li><li> After operation "A 1 3": $A=[0,0,0]$, $B=[0,0,0]$ (addition is modulo 3).</li><li> After operation "A 1 3": $A=[1,1,2]$, $B=[0,0,0]$.</li><li> After operation "B 1 1": $A=[1,1,2]$, $B=[1,0,0]$.</li><li> After operation "B 2 2": $A=[1,1,2]$, $B=[1,1,0]$.</li><li> After operation "A 3 3": $A=[1,1,0]$, $B=[1,1,0]$.</li></ul>
