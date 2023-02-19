## Description

<div><p>Consider every tree (connected undirected acyclic graph) with $n$ vertices (<span class="tex-font-style-bf">$n$ is odd</span>, vertices numbered from $1$ to $n$), and for each $2 \le i \le n$ the $i$-th vertex is adjacent to exactly one vertex with a smaller index.</p><p>For each $i$ ($1 \le i \le n$) calculate the number of trees for which the $i$-th vertex will be the centroid. The answer can be huge, output it modulo $998\,244\,353$.</p><p>A vertex is called a centroid if its removal splits the tree into subtrees with at most $(n-1)/2$ vertices each.</p></div><div class="input-specification"><p>The first line contains an odd integer $n$ ($3 \le n &lt; 2 \cdot 10^5$, $n$ is odd) — the number of the vertices in the tree.</p></div><div class="output-specification"><p>Print $n$ integers in a single line, the $i$-th integer is the answer for the $i$-th vertex (modulo $998\,244\,353$).</p></div>

## Input

<p>The first line contains an odd integer $n$ ($3 \le n &lt; 2 \cdot 10^5$, $n$ is odd) — the number of the vertices in the tree.</p>

## Output

<p>Print $n$ integers in a single line, the $i$-th integer is the answer for the $i$-th vertex (modulo $998\,244\,353$).</p>





```input1
3
```




```input2
5
```




```input3
7
```




```output1
1 1 0
```




```output2
10 10 4 0 0
```




```output3
276 276 132 36 0 0 0
```



## Note

<p>Example $1$: there are two possible trees: with edges $(1-2)$, and $(1-3)$ — here the centroid is $1$; and with edges $(1-2)$, and $(2-3)$ — here the centroid is $2$. So the answer is $1, 1, 0$.</p><p>Example $2$: there are $24$ possible trees, for example with edges $(1-2)$, $(2-3)$, $(3-4)$, and $(4-5)$. Here the centroid is $3$.</p>
