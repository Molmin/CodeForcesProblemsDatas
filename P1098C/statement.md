## Description

<div><p>Misha walked through the snowy forest and he was so fascinated by the trees to decide to draw his own tree!</p><p>Misha would like to construct a rooted tree with $n$ vertices, indexed from 1 to $n$, where the root has index 1. Every other vertex has a <span class="tex-font-style-it">parent</span> $p_i$, and $i$ is called a <span class="tex-font-style-it">child</span> of vertex $p_i$. Vertex $u$ belongs to the <span class="tex-font-style-it">subtree</span> of vertex $v$ iff $v$ is reachable from $u$ while iterating over the parents ($u$, $p_{u}$, $p_{p_{u}}$, ...). Clearly, $v$ belongs to its own subtree, and the number of vertices in the subtree is called the <span class="tex-font-style-it">size</span> of the subtree. Misha is only interested in trees where every vertex belongs to the subtree of vertex $1$.</p><p>Below there is a tree with $6$ vertices. The subtree of vertex $2$ contains vertices $2$, $3$, $4$, $5$. Hence the size of its subtree is $4$. </p><center> <img class="tex-graphics" src="file://sieIZp7V.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>The <span class="tex-font-style-it">branching coefficient</span> of the tree is defined as the maximum number of children in any vertex. For example, for the tree above the branching coefficient equals $2$. Your task is to construct a tree with $n$ vertices such that the sum of the subtree sizes for all vertices equals $s$, and the branching coefficient is minimum possible.</p></div><div class="input-specification"><p>The only input line contains two integers $n$ and $s$&nbsp;— the number of vertices in the tree and the desired sum of the subtree sizes ($2 \le n \le 10^5$; $1 \le s \le 10^{10}$).</p></div><div class="output-specification"><p>If the required tree does not exist, output «<span class="tex-font-style-tt">No</span>». Otherwise output «<span class="tex-font-style-tt">Yes</span>» on the first line, and in the next one output integers $p_2$, $p_3$, ..., $p_n$, where $p_i$ denotes the parent of vertex $i$.</p></div>

## Input

<p>The only input line contains two integers $n$ and $s$&nbsp;— the number of vertices in the tree and the desired sum of the subtree sizes ($2 \le n \le 10^5$; $1 \le s \le 10^{10}$).</p>

## Output

<p>If the required tree does not exist, output «<span class="tex-font-style-tt">No</span>». Otherwise output «<span class="tex-font-style-tt">Yes</span>» on the first line, and in the next one output integers $p_2$, $p_3$, ..., $p_n$, where $p_i$ denotes the parent of vertex $i$.</p>





```input1
3 5
```




```input2
4 42
```




```input3
6 15
```




```output1
Yes
1 1
```




```output2
No
```




```output3
Yes
1 2 3 1 5
```



## Note

<p>Below one can find one of the possible solutions for the first sample case. The sum of subtree sizes equals $3 + 1 + 1 = 5$, and the branching coefficient equals $2$.</p><center> <img class="tex-graphics" src="file://fBCjzGam.png" style="max-width: 100.0%;max-height: 100.0%;" width="378px"> </center><p>Below one can find one of the possible solutions for the third sample case. The sum of subtree sizes equals $6 + 3 + 2 + 1 + 2 + 1 = 15$, and the branching coefficient equals $2$.</p><center> <img class="tex-graphics" src="file://qnF2O080.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
