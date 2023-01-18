## Description

<div><p>During the programming classes Vasya was assigned a difficult problem. However, he doesn't know how to code and was unable to find the solution in the Internet, so he asks you to help.</p><p>You are given a sequence $a$, consisting of $n$ <span class="tex-font-style-bf">distinct</span> integers, that is used to construct the binary search tree. Below is the formal description of the construction process.</p><ol> <li> First element $a_1$ becomes the root of the tree. </li><li> Elements $a_2, a_3, \ldots, a_n$ are added one by one. To add element $a_i$ one needs to traverse the tree starting from the root and using the following rules: <ol> <li> The pointer to the current node is set to the root. </li><li> If $a_i$ is greater than the value in the current node, then its right child becomes the current node. Otherwise, the left child of the current node becomes the new current node. </li><li> If at some point there is no required child, the new node is created, it is assigned value $a_i$ and becomes the corresponding child of the current node. </li></ol> </li></ol></div><div class="input-specification"><p>The first line of the input contains a single integer $n$ ($2 \leq n \leq 100\,000$)&nbsp;— the length of the sequence $a$.</p><p>The second line contains $n$ distinct integers $a_i$ ($1 \leq a_i \leq 10^9$)&nbsp;— the sequence $a$ itself.</p></div><div class="output-specification"><p>Output $n - 1$ integers. For all $i &gt; 1$ print the value written in the node that is the parent of the node with value $a_i$ in it.</p></div>

## Input

<p>The first line of the input contains a single integer $n$ ($2 \leq n \leq 100\,000$)&nbsp;— the length of the sequence $a$.</p><p>The second line contains $n$ distinct integers $a_i$ ($1 \leq a_i \leq 10^9$)&nbsp;— the sequence $a$ itself.</p>

## Output

<p>Output $n - 1$ integers. For all $i &gt; 1$ print the value written in the node that is the parent of the node with value $a_i$ in it.</p>





```input1
3
1 2 3

```




```input2
5
4 2 3 1 6

```




```output1
1 2

```




```output2
4 2 2 4

```


