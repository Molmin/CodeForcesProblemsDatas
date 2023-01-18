## Description

<div><p>Ildar is the algorithm teacher of William and Harris. Today, Ildar is teaching Cartesian Tree. However, Harris is sick, so Ildar is only teaching William.</p><p>A cartesian tree is a rooted tree, that can be constructed from a sequence of distinct integers. We build the cartesian tree as follows:</p><ol><li> If the sequence is empty, return an empty tree;</li><li> Let the position of the <span class="tex-font-style-bf">maximum</span> element be $x$;</li><li> Remove element on the position $x$ from the sequence and break it into the left part and the right part (which might be empty) (not actually removing it, just taking it away temporarily);</li><li> Build cartesian tree for each part;</li><li> Create a new vertex for the element, that was on the position $x$ which will serve as the root of the new tree. Then, for the root of the left part and right part, if exists, will become the children for this vertex;</li><li> Return the tree we have gotten.</li></ol><p>For example, this is the cartesian tree for the sequence $4, 2, 7, 3, 5, 6, 1$:</p><center> <img class="tex-graphics" src="file://k0jE32Ei.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>After teaching what the cartesian tree is, Ildar has assigned homework. He starts with an empty sequence $a$.</p><p>In the $i$-th round, he inserts an element with value $i$ somewhere in $a$. Then, he asks a question: what is the sum of the sizes of the subtrees for every node in the cartesian tree for the current sequence $a$?</p><p>Node $v$ is in the node $u$ subtree if and only if $v = u$ or $v$ is in the subtree of one of the vertex $u$ children. The size of the subtree of node $u$ is the number of nodes $v$ such that $v$ is in the subtree of $u$.</p><p>Ildar will do $n$ rounds in total. The homework is the sequence of answers to the $n$ questions.</p><p>The next day, Ildar told Harris that he has to complete the homework as well. Harris obtained the final state of the sequence $a$ from William. However, he has no idea how to find the answers to the $n$ questions. Help Harris!</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($1 \le n \le 150000$).</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le n$). It is guarenteed that each integer from $1$ to $n$ appears in the sequence exactly once.</p></div><div class="output-specification"><p>Print $n$ lines, $i$-th line should contain a single integer &nbsp;— the answer to the $i$-th question.</p></div>

## Input

<p>The first line contains a single integer $n$ ($1 \le n \le 150000$).</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le n$). It is guarenteed that each integer from $1$ to $n$ appears in the sequence exactly once.</p>

## Output

<p>Print $n$ lines, $i$-th line should contain a single integer &nbsp;— the answer to the $i$-th question.</p>





```input1
5
2 4 1 5 3
```




```input2
6
1 2 4 5 6 3
```




```output1
1
3
6
8
11
```




```output2
1
3
6
8
12
17
```



## Note

<p>After the first round, the sequence is $1$. The tree is</p><center> <img class="tex-graphics" src="file://a8tT5x74.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>The answer is $1$.</p><p>After the second round, the sequence is $2, 1$. The tree is</p><center> <img class="tex-graphics" src="file://zFx1cLMs.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>The answer is $2+1=3$.</p><p>After the third round, the sequence is $2, 1, 3$. The tree is</p><center> <img class="tex-graphics" src="file://AIu4wtUU.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>The answer is $2+1+3=6$.</p><p>After the fourth round, the sequence is $2, 4, 1, 3$. The tree is</p><center> <img class="tex-graphics" src="file://Uvoqk9X8.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>The answer is $1+4+1+2=8$.</p><p>After the fifth round, the sequence is $2, 4, 1, 5, 3$. The tree is</p><center> <img class="tex-graphics" src="file://jdMfXuan.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>The answer is $1+3+1+5+1=11$.</p>
