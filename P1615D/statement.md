## Description

<div><p>'Twas the night before Christmas, and Santa's frantically setting up his new Christmas tree! There are $n$ nodes in the tree, connected by $n-1$ edges. On each edge of the tree, there's a set of Christmas lights, which can be represented by an integer in binary representation.</p><center> <img class="tex-graphics" src="file://jJigNWIn.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>He has $m$ elves come over and admire his tree. Each elf is assigned two nodes, $a$ and $b$, and that elf looks at all lights on the simple path between the two nodes. After this, the elf's favorite number becomes the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#XOR">bitwise XOR</a> of the values of the lights on the edges in that path.</p><p>However, the North Pole has been recovering from a nasty bout of flu. Because of this, Santa forgot some of the configurations of lights he had put on the tree, and he has already left the North Pole! Fortunately, the elves came to the rescue, and each one told Santa what pair of nodes he was assigned $(a_i, b_i)$, as well as <span class="tex-font-style-bf">the parity</span> of the number of set bits in his favorite number. In other words, he remembers whether the number of $1$'s when his favorite number is written in binary is <span class="tex-font-style-bf">odd or even</span>.</p><p>Help Santa determine if it's possible that the memories are consistent, and if it is, remember what his tree looked like, and maybe you'll go down in history!</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \leq t \leq 2 \cdot 10^4$)&nbsp;— the number of test cases. Then $t$ cases follow.</p><p>The first line of each test case contains two integers, $n$ and $m$ ($2 \leq n \leq 2 \cdot 10^5$; $1 \leq m \leq 2 \cdot 10^5$)&nbsp;— the size of tree and the number of elves respectively.</p><p>The next $n-1$ lines of each test case each contains three integers, $x$, $y$, and $v$ ($1 \leq x, y \leq n$; $-1 \leq v &lt; 2^{30}$)&nbsp;— meaning that there's an edge between nodes $x$ and $y$. If </p><ul> <li> $v = -1$: Santa doesn't remember what the set of lights were on for this edge. </li><li> $v \geq 0$: The set of lights on the edge is $v$. </li></ul><p>The next $m$ lines of each test case each contains three integers, $a$, $b$, and $p$ ($1 \leq a, b \leq n$; $a \neq b$; $0 \leq p \leq 1$)&nbsp;— the nodes that the elf was assigned to, and the <span class="tex-font-style-bf">parity</span> of the number of set bits in the elf's favorite number.</p><p>It is guaranteed that the sum of all $n$ and the sum of all $m$ don't exceed $2 \cdot 10^5$ each.</p><p>It is guaranteed that the given edges form a tree.</p></div><div class="output-specification"><p>For each test case, first print either <span class="tex-font-style-tt">YES</span> or <span class="tex-font-style-tt">NO</span> (in any case), whether there's a tree consistent with Santa's memory or not. </p><p>If the answer is <span class="tex-font-style-tt">YES</span>, print $n-1$ lines each containing three integers: $x$, $y$, and $v$ ($1 \le x, y \le n$; $0 \le v &lt; 2^{30}$)&nbsp;— the edge and the integer on that edge. The set of edges must be the same as in the input, and if the value of some edge was specified earlier, it can not change. You can print the edges in any order.</p><p>If there are multiple answers, print any.</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \leq t \leq 2 \cdot 10^4$)&nbsp;— the number of test cases. Then $t$ cases follow.</p><p>The first line of each test case contains two integers, $n$ and $m$ ($2 \leq n \leq 2 \cdot 10^5$; $1 \leq m \leq 2 \cdot 10^5$)&nbsp;— the size of tree and the number of elves respectively.</p><p>The next $n-1$ lines of each test case each contains three integers, $x$, $y$, and $v$ ($1 \leq x, y \leq n$; $-1 \leq v &lt; 2^{30}$)&nbsp;— meaning that there's an edge between nodes $x$ and $y$. If </p><ul> <li> $v = -1$: Santa doesn't remember what the set of lights were on for this edge. </li><li> $v \geq 0$: The set of lights on the edge is $v$. </li></ul><p>The next $m$ lines of each test case each contains three integers, $a$, $b$, and $p$ ($1 \leq a, b \leq n$; $a \neq b$; $0 \leq p \leq 1$)&nbsp;— the nodes that the elf was assigned to, and the <span class="tex-font-style-bf">parity</span> of the number of set bits in the elf's favorite number.</p><p>It is guaranteed that the sum of all $n$ and the sum of all $m$ don't exceed $2 \cdot 10^5$ each.</p><p>It is guaranteed that the given edges form a tree.</p>

## Output

<p>For each test case, first print either <span class="tex-font-style-tt">YES</span> or <span class="tex-font-style-tt">NO</span> (in any case), whether there's a tree consistent with Santa's memory or not. </p><p>If the answer is <span class="tex-font-style-tt">YES</span>, print $n-1$ lines each containing three integers: $x$, $y$, and $v$ ($1 \le x, y \le n$; $0 \le v &lt; 2^{30}$)&nbsp;— the edge and the integer on that edge. The set of edges must be the same as in the input, and if the value of some edge was specified earlier, it can not change. You can print the edges in any order.</p><p>If there are multiple answers, print any.</p>





```input1
4
6 5
1 2 -1
1 3 1
4 2 7
6 3 0
2 5 -1
2 3 1
2 5 0
5 6 1
6 1 1
4 5 1
5 3
1 2 -1
1 3 -1
1 4 1
4 5 -1
2 4 0
3 4 1
2 3 1
3 3
1 2 -1
1 3 -1
1 2 0
1 3 1
2 3 0
2 1
1 2 1
1 2 0
```




```output1
YES
1 2 0
1 3 1
2 4 7
3 6 0
2 5 0
YES
1 2 1
1 3 0
1 4 1
4 5 1
NO
NO
```



## Note

<p>The first test case is the image in the statement.</p><p>One possible answer is assigning the value of the edge $(1, 2)$ to $5$, and the value of the edge $(2, 5)$ to $3$. This is correct because: </p><ul> <li> The first elf goes from node $2$ to node $3$. This elf's favorite number is $4$, so he remembers the value $1$ (as $4$ has an odd number of $1$ bits in its binary representation). </li><li> The second elf goes from node $2$ to node $5$. This elf's favorite number is $3$, so he remembers the value $0$ (as $3$ has an even number of $1$ bits in its binary representation). </li><li> The third elf goes from node $5$ to node $6$. This elf's favorite number is $7$, so he remembers the value $1$ (as $7$ has an odd number of $1$ bits in its binary representation). </li><li> The fourth elf goes from node $6$ to node $1$. This elf's favorite number is $1$, so he remembers the value $1$ (as $1$ has an odd number of $1$ bits in its binary representation). </li><li> The fifth elf goes from node $4$ to node $5$. This elf's favorite number is $4$, so he remembers the number $1$ (as $4$ has an odd number of $1$ bits in its binary representation). </li></ul><p>Note that there are other possible answers.</p>
