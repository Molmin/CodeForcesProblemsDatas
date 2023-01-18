## Description

<div><p>You are given an array $a$ consisting of $n$ integers. You can perform the following operations with it: </p><ol> <li> Choose some positions $i$ and $j$ ($1 \le i, j \le n, i \ne j$), write the value of $a_i \cdot a_j$ into the $j$-th cell and <span class="tex-font-style-bf">remove the number</span> from the $i$-th cell; </li><li> Choose some position $i$ and <span class="tex-font-style-bf">remove the number</span> from the $i$-th cell (this operation can be performed <span class="tex-font-style-bf">no more than once and at any point of time, not necessarily in the beginning</span>). </li></ol><p>The number of elements decreases by one after each operation. However, the indexing of positions stays the same. Deleted numbers can't be used in the later operations.</p><p>Your task is to perform exactly $n - 1$ operations with the array in such a way that the only number that remains in the array is maximum possible. This number can be rather large, so instead of printing it you need to print <span class="tex-font-style-bf">any</span> sequence of operations which leads to this maximum number. Read the output format to understand what exactly you need to print.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($2 \le n \le 2 \cdot 10^5$) — the number of elements in the array.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($-10^9 \le a_i \le 10^9$) — the elements of the array.</p></div><div class="output-specification"><p>Print $n - 1$ lines. The $k$-th line should contain one of the two possible operations.</p><p>The operation of the first type should look like this: $1~ i_k~ j_k$, where $1$ is the type of operation, $i_k$ and $j_k$ are the positions of the chosen elements.</p><p>The operation of the second type should look like this: $2~ i_k$, where $2$ is the type of operation, $i_k$ is the position of the chosen element. Note that there should be no more than one such operation.</p><p>If there are multiple possible sequences of operations leading to the maximum number — print <span class="tex-font-style-bf">any</span> of them.</p></div>

## Input

<p>The first line contains a single integer $n$ ($2 \le n \le 2 \cdot 10^5$) — the number of elements in the array.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($-10^9 \le a_i \le 10^9$) — the elements of the array.</p>

## Output

<p>Print $n - 1$ lines. The $k$-th line should contain one of the two possible operations.</p><p>The operation of the first type should look like this: $1~ i_k~ j_k$, where $1$ is the type of operation, $i_k$ and $j_k$ are the positions of the chosen elements.</p><p>The operation of the second type should look like this: $2~ i_k$, where $2$ is the type of operation, $i_k$ is the position of the chosen element. Note that there should be no more than one such operation.</p><p>If there are multiple possible sequences of operations leading to the maximum number — print <span class="tex-font-style-bf">any</span> of them.</p>





```input1
5
5 -2 0 1 -3

```




```input2
5
5 2 0 4 0

```




```input3
2
2 -1

```




```input4
4
0 -10 0 0

```




```input5
4
0 0 0 0

```




```output1
2 3
1 1 2
1 2 4
1 4 5

```




```output2
1 3 5
2 5
1 1 2
1 2 4

```




```output3
2 2

```




```output4
1 1 2
1 2 3
1 3 4

```




```output5
1 1 2
1 2 3
1 3 4

```



## Note

<p>Let <span class="tex-font-style-tt">X</span> be the removed number in the array. Let's take a look at all the examples:</p><p>The first example has, for example, the following sequence of transformations of the array: $[5, -2, 0, 1, -3] \to [5, -2, X, 1, -3] \to [X, -10, X, 1, -3] \to$ $[X, X, X, -10, -3] \to [X, X, X, X, 30]$. Thus, the maximum answer is $30$. <span class="tex-font-style-bf">Note, that other sequences that lead to the answer $30$ are also correct</span>.</p><p>The second example has, for example, the following sequence of transformations of the array: $[5, 2, 0, 4, 0] \to [5, 2, X, 4, 0] \to [5, 2, X, 4, X] \to [X, 10, X, 4, X] \to$ $[X, X, X, 40, X]$. The following answer is also allowed: </p><pre class="verbatim"><br>1 5 3<br>1 4 2<br>1 2 1<br>2 3<br></pre><p>Then the sequence of transformations of the array will look like this: $[5, 2, 0, 4, 0] \to [5, 2, 0, 4, X] \to [5, 8, 0, X, X] \to [40, X, 0, X, X] \to$ $[40, X, X, X, X]$.</p><p>The third example can have the following sequence of transformations of the array: $[2, -1] \to [2, X]$.</p><p>The fourth example can have the following sequence of transformations of the array: $[0, -10, 0, 0] \to [X, 0, 0, 0] \to [X, X, 0, 0] \to [X, X, X, 0]$.</p><p>The fifth example can have the following sequence of transformations of the array: $[0, 0, 0, 0] \to [X, 0, 0, 0] \to [X, X, 0, 0] \to [X, X, X, 0]$.</p>
