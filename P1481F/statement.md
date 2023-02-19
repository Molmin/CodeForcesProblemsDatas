## Description

<div><p>Kilani and Abd are neighbors for 3000 years, but then the day came and Kilani decided to move to another house. As a farewell gift, Kilani is going to challenge Abd with a problem written by their other neighbor with the same name Abd.</p><center> <img class="tex-graphics" src="file://Rzd6In2E.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>The problem is:</p><p>You are given a connected tree rooted at node $1$.</p><p>You should assign a character <span class="tex-font-style-tt">a</span> or <span class="tex-font-style-tt">b</span> to every node in the tree so that the total number of <span class="tex-font-style-tt">a</span>'s is equal to $x$ and the total number of <span class="tex-font-style-tt">b</span>'s is equal to $n - x$.</p><p>Let's define a string for each node $v$ of the tree as follows: </p><ul> <li> if $v$ is root then the string is just one character assigned to $v$: </li><li> otherwise, let's take a string defined for the $v$'s parent $p_v$ and add to the end of it a character assigned to $v$. </li></ul><p>You should assign every node a character in a way that <span class="tex-font-style-bf">minimizes the number of distinct strings</span> among the strings of all nodes.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $x$ ($1 \leq n \leq 10^5$; $0 \leq x \leq n$)&nbsp;— the number of vertices in the tree the number of <span class="tex-font-style-tt">a</span>'s.</p><p>The second line contains $n - 1$ integers $p_2, p_3, \dots, p_{n}$ ($1 \leq p_i \leq n$; $p_i \neq i$), where $p_i$ is the parent of node $i$.</p><p>It is guaranteed that the input describes a connected tree.</p></div><div class="output-specification"><p>In the first line, print the minimum possible total number of distinct strings.</p><p>In the second line, print $n$ characters, where all characters are either <span class="tex-font-style-tt">a</span> or <span class="tex-font-style-tt">b</span> and the $i$-th character is the character assigned to the $i$-th node.</p><p>Make sure that the total number of <span class="tex-font-style-tt">a</span>'s is equal to $x$ and the total number of <span class="tex-font-style-tt">b</span>'s is equal to $n - x$.</p><p>If there is more than one answer you can print any of them.</p></div>

## Input

<p>The first line contains two integers $n$ and $x$ ($1 \leq n \leq 10^5$; $0 \leq x \leq n$)&nbsp;— the number of vertices in the tree the number of <span class="tex-font-style-tt">a</span>'s.</p><p>The second line contains $n - 1$ integers $p_2, p_3, \dots, p_{n}$ ($1 \leq p_i \leq n$; $p_i \neq i$), where $p_i$ is the parent of node $i$.</p><p>It is guaranteed that the input describes a connected tree.</p>

## Output

<p>In the first line, print the minimum possible total number of distinct strings.</p><p>In the second line, print $n$ characters, where all characters are either <span class="tex-font-style-tt">a</span> or <span class="tex-font-style-tt">b</span> and the $i$-th character is the character assigned to the $i$-th node.</p><p>Make sure that the total number of <span class="tex-font-style-tt">a</span>'s is equal to $x$ and the total number of <span class="tex-font-style-tt">b</span>'s is equal to $n - x$.</p><p>If there is more than one answer you can print any of them.</p>





```input1
9 3
1 2 2 4 4 4 3 1
```




```output1
4
aabbbbbba
```



## Note

<p>The tree from the sample is shown below:</p><center> <img class="tex-graphics" src="file://m6G3t0nJ.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>The tree after assigning characters to every node (according to the output) is the following:</p><center> <img class="tex-graphics" src="file://kaxCky83.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Strings for all nodes are the following: </p><ul> <li> string of node $1$ is: <span class="tex-font-style-tt">a</span> </li><li> string of node $2$ is: <span class="tex-font-style-tt">aa</span> </li><li> string of node $3$ is: <span class="tex-font-style-tt">aab</span> </li><li> string of node $4$ is: <span class="tex-font-style-tt">aab</span> </li><li> string of node $5$ is: <span class="tex-font-style-tt">aabb</span> </li><li> string of node $6$ is: <span class="tex-font-style-tt">aabb</span> </li><li> string of node $7$ is: <span class="tex-font-style-tt">aabb</span> </li><li> string of node $8$ is: <span class="tex-font-style-tt">aabb</span> </li><li> string of node $9$ is: <span class="tex-font-style-tt">aa</span> </li></ul><p>The set of unique strings is $\{\text{a}, \text{aa}, \text{aab}, \text{aabb}\}$, so the number of distinct strings is $4$.</p>
