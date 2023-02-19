## Description

<div><p>CQXYM found a rectangle $A$ of size $n \times m$. There are $n$ rows and $m$ columns of blocks. Each block of the rectangle is an obsidian block or empty. CQXYM can change an obsidian block to an empty block or an empty block to an obsidian block in one operation.</p><p>A rectangle $M$ size of $a \times b$ is called a portal if and only if it satisfies the following conditions:</p><ul> <li> $a \geq 5,b \geq 4$. </li><li> For all $1 &lt; x &lt; a$, blocks $M_{x,1}$ and $M_{x,b}$ are obsidian blocks. </li><li> For all $1 &lt; x &lt; b$, blocks $M_{1,x}$ and $M_{a,x}$ are obsidian blocks. </li><li> For all $1&lt;x&lt;a,1&lt;y&lt;b$, block $M_{x,y}$ is an empty block. </li><li> $M_{1, 1}, M_{1, b}, M_{a, 1}, M_{a, b}$ <span class="tex-font-style-bf">can be any type</span>. </li></ul> Note that the there must be $a$ rows and $b$ columns, not $b$ rows and $a$ columns.<p><span class="tex-font-style-bf">Note that corners can be any type</span></p><p>CQXYM wants to know the minimum number of operations he needs to make at least one sub-rectangle a portal.</p></div><div class="input-specification"><p>The first line contains an integer $t$ ($t \geq 1$), which is the number of test cases.</p><p>For each test case, the first line contains two integers $n$ and $m$ ($5 \le n \le 400$, $4 \le m \le 400$). </p><p>Then $n$ lines follow, each line contains $m$ characters $0$ or $1$. If the $j$-th character of $i$-th line is $0$, block $A_{i,j}$ is an empty block. Otherwise, block $A_{i,j}$ is an obsidian block.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $400$.</p><p>It is guaranteed that the sum of $m$ over all test cases does not exceed $400$.</p></div><div class="output-specification"><p>Output $t$ answers, and each answer in a line.</p></div>

## Input

<p>The first line contains an integer $t$ ($t \geq 1$), which is the number of test cases.</p><p>For each test case, the first line contains two integers $n$ and $m$ ($5 \le n \le 400$, $4 \le m \le 400$). </p><p>Then $n$ lines follow, each line contains $m$ characters $0$ or $1$. If the $j$-th character of $i$-th line is $0$, block $A_{i,j}$ is an empty block. Otherwise, block $A_{i,j}$ is an obsidian block.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $400$.</p><p>It is guaranteed that the sum of $m$ over all test cases does not exceed $400$.</p>

## Output

<p>Output $t$ answers, and each answer in a line.</p>





```input1
1
5 4
1000
0000
0110
0000
0001
```




```input2
1
9 9
001010001
101110100
000010011
100000001
101010101
110001111
000001111
111100000
000110000
```




```output1
12
```




```output2
5
```



## Note

<p>In the first test case, the final portal is like this:</p><pre class="verbatim"><br>1110<br>1001<br>1001<br>1001<br>0111<br></pre>
