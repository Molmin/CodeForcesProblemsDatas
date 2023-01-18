## Description

<div><p>Find out if it is possible to partition the first $n$ positive integers into two <span class="tex-font-style-bf">non-empty</span> disjoint sets $S_1$ and $S_2$ such that:</p><center>$\mathrm{gcd}(\mathrm{sum}(S_1), \mathrm{sum}(S_2)) &gt; 1$ </center><p>Here $\mathrm{sum}(S)$ denotes the sum of all elements present in set $S$ and $\mathrm{gcd}$ means the<a href="https://en.wikipedia.org/wiki/Greatest_common_divisor">greatest common divisor</a>.</p><p>Every integer number from $1$ to $n$ should be present in <span class="tex-font-style-bf">exactly one</span> of $S_1$ or $S_2$.</p></div><div class="input-specification"><p>The only line of the input contains a single integer $n$ ($1 \le n \le 45\,000$)</p></div><div class="output-specification"><p>If such partition doesn't exist, print "No" (quotes for clarity).</p><p>Otherwise, print "Yes" (quotes for clarity), followed by two lines, describing $S_1$ and $S_2$ respectively.</p><p>Each set description starts with the set size, followed by the elements of the set in any order. Each set must be non-empty.</p><p>If there are multiple possible partitions&nbsp;— print any of them.</p></div>

## Input

<p>The only line of the input contains a single integer $n$ ($1 \le n \le 45\,000$)</p>

## Output

<p>If such partition doesn't exist, print "No" (quotes for clarity).</p><p>Otherwise, print "Yes" (quotes for clarity), followed by two lines, describing $S_1$ and $S_2$ respectively.</p><p>Each set description starts with the set size, followed by the elements of the set in any order. Each set must be non-empty.</p><p>If there are multiple possible partitions&nbsp;— print any of them.</p>





```input1
1

```




```input2
3

```




```output1
No
```




```output2
Yes
1 2
2 1 3 

```



## Note

<p>In the first example, there is no way to partition a single number into two non-empty sets, hence the answer is "No".</p><p>In the second example, the sums of the sets are $2$ and $4$ respectively. The $\mathrm{gcd}(2, 4) = 2 &gt; 1$, hence that is one of the possible answers.</p>
