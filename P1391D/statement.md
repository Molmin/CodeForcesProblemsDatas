## Description

<div><p>A binary matrix is called <span class="tex-font-style-bf">good</span> if every <span class="tex-font-style-bf">even</span> length square sub-matrix has an <span class="tex-font-style-bf">odd</span> number of ones. </p><p>Given a binary matrix $a$ consisting of $n$ rows and $m$ columns, determine the minimum number of cells you need to change to make it good, or report that there is no way to make it good at all. </p><p>All the terms above have their usual meanings&nbsp;— refer to the Notes section for their formal definitions. </p></div><div class="input-specification"><p>The first line of input contains two integers $n$ and $m$ ($1 \leq n \leq m \leq 10^6$ and $n\cdot m \leq 10^6$) &nbsp;— the number of rows and columns in $a$, respectively. </p><p>The following $n$ lines each contain $m$ characters, each of which is one of <span class="tex-font-style-tt">0</span> and <span class="tex-font-style-tt">1</span>. If the $j$-th character on the $i$-th line is <span class="tex-font-style-tt">1</span>, then $a_{i,j} = 1$. Similarly, if the $j$-th character on the $i$-th line is <span class="tex-font-style-tt">0</span>, then $a_{i,j} = 0$.</p></div><div class="output-specification"><p>Output the minimum number of cells you need to change to make $a$ good, or output $-1$ if it's not possible at all.</p></div>

## Input

<p>The first line of input contains two integers $n$ and $m$ ($1 \leq n \leq m \leq 10^6$ and $n\cdot m \leq 10^6$) &nbsp;— the number of rows and columns in $a$, respectively. </p><p>The following $n$ lines each contain $m$ characters, each of which is one of <span class="tex-font-style-tt">0</span> and <span class="tex-font-style-tt">1</span>. If the $j$-th character on the $i$-th line is <span class="tex-font-style-tt">1</span>, then $a_{i,j} = 1$. Similarly, if the $j$-th character on the $i$-th line is <span class="tex-font-style-tt">0</span>, then $a_{i,j} = 0$.</p>

## Output

<p>Output the minimum number of cells you need to change to make $a$ good, or output $-1$ if it's not possible at all.</p>





```input1
3 3
101
001
110
```




```input2
7 15
000100001010010
100111010110001
101101111100100
010000111111010
111010010100001
000011001111101
111111011010011
```




```output1
2
```




```output2
-1
```



## Note

<p>In the first case, changing $a_{1,1}$ to $0$ and $a_{2,2}$ to $1$ is enough. </p><p>You can verify that there is no way to make the matrix in the second case good. </p><p>Some definitions&nbsp;— </p><ul> <li> A binary matrix is one in which every element is either $1$ or $0$. </li><li> A sub-matrix is described by $4$ parameters&nbsp;— $r_1$, $r_2$, $c_1$, and $c_2$; here, $1 \leq r_1 \leq r_2 \leq n$ and $1 \leq c_1 \leq c_2 \leq m$. </li><li> This sub-matrix contains all elements $a_{i,j}$ that satisfy both $r_1 \leq i \leq r_2$ and $c_1 \leq j \leq c_2$. </li><li> A sub-matrix is, further, called an even length square if $r_2-r_1 = c_2-c_1$ and $r_2-r_1+1$ is divisible by $2$. </li></ul>
