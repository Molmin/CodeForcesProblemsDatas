## Description

<div><p>The Main Martian Tree grows on Mars. It is a binary tree (a rooted tree, with no more than two sons at each vertex) with $n$ vertices, where the root vertex has the number $1$. Its fruits are the Main Martian Fruits. It's summer now, so this tree does not have any fruit yet.</p><p>Autumn is coming soon, and leaves and branches will begin to fall off the tree. It is clear, that if a vertex falls off the tree, then its entire subtree will fall off too. In addition, the root will remain on the tree. Formally: the tree will have some connected subset of vertices containing the root.</p><p>After that, the fruits will grow on the tree (only at those vertices which remain). Exactly $x$ fruits will grow in the root. The number of fruits in each remaining vertex will be not less than the sum of the numbers of fruits in the remaining sons of this vertex. It is allowed, that some vertices will not have any fruits.</p><p>Natasha wondered how many tree configurations can be after the described changes. Since this number can be very large, output it modulo $998244353$.</p><p>Two configurations of the resulting tree are considered different if one of these two conditions is true:</p><ul><li> they have different subsets of remaining vertices;</li><li> they have the same subset of remaining vertices, but there is a vertex in this subset where they have a different amount of fruits.</li></ul></div><div class="input-specification"><p>The first line contains two integers: $n$ and $x$ ($1 \le n \le 10^5$, $0 \le x \le 10^{18}$)&nbsp;— the size of the tree and the number of fruits in the root.</p><p>The $i$-th of the following $(n-1)$ lines contains two integers $a_i$ and $b_i$ ($1 \le a_i, b_i \le n$)&nbsp;— vertices connected by the $i$-th edge of the tree.</p><p>It is guaranteed that the input data describes a correct binary tree with the root at the vertex $1$.</p></div><div class="output-specification"><p>Print one number&nbsp;— the number of configurations of the resulting tree modulo $998244353$.</p></div>

## Input

<p>The first line contains two integers: $n$ and $x$ ($1 \le n \le 10^5$, $0 \le x \le 10^{18}$)&nbsp;— the size of the tree and the number of fruits in the root.</p><p>The $i$-th of the following $(n-1)$ lines contains two integers $a_i$ and $b_i$ ($1 \le a_i, b_i \le n$)&nbsp;— vertices connected by the $i$-th edge of the tree.</p><p>It is guaranteed that the input data describes a correct binary tree with the root at the vertex $1$.</p>

## Output

<p>Print one number&nbsp;— the number of configurations of the resulting tree modulo $998244353$.</p>





```input1
3 2
1 2
1 3

```




```input2
2 5
1 2

```




```input3
4 10
1 2
1 3
3 4

```




```output1
13

```




```output2
7

```




```output3
441

```



## Note

<p>Consider the first example. <img class="tex-graphics" src="file://IH3yNjpI.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>There are $2$ fruits at the vertex $1$. The following $13$ options are possible:</p><ul><li> there is no vertex $2$, there is no vertex $3$; <img class="tex-graphics" src="file://3gamx6YN.png" style="max-width: 100.0%;max-height: 100.0%;"></li><li> there is no vertex $2$, there are no fruits at the vertex $3$; <img class="tex-graphics" src="file://ZZAtHLbC.png" style="max-width: 100.0%;max-height: 100.0%;"></li><li> there is no vertex $2$, there is $1$ fruit at the vertex $3$; <img class="tex-graphics" src="file://YwPESm36.png" style="max-width: 100.0%;max-height: 100.0%;"></li><li> there is no vertex $2$, there are $2$ fruits at the vertex $3$; <img class="tex-graphics" src="file://7yCQdoFh.png" style="max-width: 100.0%;max-height: 100.0%;"></li><li> there are no fruits at the vertex $2$, there is no vertex $3$; <img class="tex-graphics" src="file://lc7ARnhw.png" style="max-width: 100.0%;max-height: 100.0%;"></li><li> there are no fruits at the vertex $2$, there are no fruits at the vertex $3$; <img class="tex-graphics" src="file://aXenR4i9.png" style="max-width: 100.0%;max-height: 100.0%;"></li><li> there are no fruits at the vertex $2$, there is $1$ fruit at the vertex $3$; <img class="tex-graphics" src="file://mB5xklG4.png" style="max-width: 100.0%;max-height: 100.0%;"></li><li> there are no fruits at the vertex $2$, there are $2$ fruits at the vertex $3$; <img class="tex-graphics" src="file://jxcgf94F.png" style="max-width: 100.0%;max-height: 100.0%;"></li><li> there is $1$ fruit at the vertex $2$, there is no vertex $3$; <img class="tex-graphics" src="file://LJjKX3JZ.png" style="max-width: 100.0%;max-height: 100.0%;"></li><li> there is $1$ fruit at the vertex $2$, there are no fruits at the vertex $3$; <img class="tex-graphics" src="file://CnirykzX.png" style="max-width: 100.0%;max-height: 100.0%;"></li><li> there is $1$ fruit at the vertex $2$, there is $1$ fruit at the vertex $3$; <img class="tex-graphics" src="file://sJo4gVLw.png" style="max-width: 100.0%;max-height: 100.0%;"></li><li> there are $2$ fruits at the vertex $2$, there is no vertex $3$; <img class="tex-graphics" src="file://VSD4thf1.png" style="max-width: 100.0%;max-height: 100.0%;"></li><li> there are $2$ fruits at the vertex $2$, there are no fruits at the vertex $3$. <img class="tex-graphics" src="file://qVmEgWQF.png" style="max-width: 100.0%;max-height: 100.0%;"></li></ul><p>Consider the second example. There are $5$ fruits at the vertex $1$. The following $7$ options are possible:</p><ul><li> there is no vertex $2$;</li><li> there are no fruits at the vertex $2$;</li><li> there is $1$ fruit at the vertex $2$;</li><li> there are $2$ fruits at the vertex $2$;</li><li> there are $3$ fruits at the vertex $2$;</li><li> there are $4$ fruits at the vertex $2$;</li><li> there are $5$ fruits at the vertex $2$.</li></ul>
