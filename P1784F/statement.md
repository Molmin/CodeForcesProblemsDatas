## Description

<div><p>Vika has a set of all consecutive positive integers from $1$ to $2n$, inclusive.</p><p>Exactly $k$ times Vika will choose and perform one of the following two actions: </p><ul> <li> take two smallest integers from her current set and remove them; </li><li> take two median integers from her current set and remove them. </li></ul><p>Recall that medians are the integers located exactly in the middle of the set if you write down its elements in increasing order. Note that Vika's set always has an even size, thus the pair of median integers is uniquely defined. For example, two median integers of the set $\{1, 5, 6, 10, 15, 16, 18, 23\}$ are $10$ and $15$.</p><p>How many different sets can Vika obtain in the end, after $k$ actions? Print this number modulo $998\,244\,353$. Two sets are considered different if some integer belongs to one of them but not to the other.</p></div><div class="input-specification"><p>The only line contains two integers $n$ and $k$ ($1 \le k \le n \le 10^6$).</p></div><div class="output-specification"><p>Print a single integer&nbsp;— the number of sets Vika can obtain in the end, modulo $998\,244\,353$.</p></div>

## Input

<p>The only line contains two integers $n$ and $k$ ($1 \le k \le n \le 10^6$).</p>

## Output

<p>Print a single integer&nbsp;— the number of sets Vika can obtain in the end, modulo $998\,244\,353$.</p>





```input1
3 1
```




```input2
3 2
```




```input3
3 3
```




```input4
7 4
```




```input5
23 8
```




```input6
100 77
```




```output1
2
```




```output2
3
```




```output3
1
```




```output4
11
```




```output5
88
```




```output6
825430474
```



## Note

<p>In the first example, Vika's initial set is $\{1, 2, 3, 4, 5, 6\}$. She can remove the minimums from it to obtain $\{3, 4, 5, 6\}$, or she can remove the medians from it to obtain $\{1, 2, 5, 6\}$.</p><p>In the second example, Vika can obtain $\{1, 6\}$, $\{3, 6\}$, or $\{5, 6\}$. For instance, Vika can obtain $\{3, 6\}$ if she removes two smallest integers first ($\{1, 2, 3, 4, 5, 6\} \rightarrow \{3, 4, 5, 6\}$), and then she removes two median integers ($\{3, 4, 5, 6\} \rightarrow \{3, 6\}$).</p><p>In the third example, regardless of Vika's choices, she'll end up with an empty set.</p>
