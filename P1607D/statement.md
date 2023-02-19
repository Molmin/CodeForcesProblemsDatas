## Description

<div><p>You are given an array of integers $a$ of length $n$. The elements of the array can be either different or the same. </p><p>Each element of the array is colored either blue or red. There are no unpainted elements in the array. One of the two operations described below can be applied to an array in a single step:</p><ul> <li> either you can select any blue element and decrease its value by $1$; </li><li> or you can select any red element and increase its value by $1$. </li></ul><p>Situations in which there are no elements of some color at all are also possible. For example, if the whole array is colored blue or red, one of the operations becomes unavailable.</p><p>Determine whether it is possible to make $0$ or more steps such that the resulting array is a permutation of numbers from $1$ to $n$?</p><p>In other words, check whether there exists a sequence of steps (possibly empty) such that after applying it, the array $a$ contains in some order all numbers from $1$ to $n$ (inclusive), each exactly once.</p></div><div class="input-specification"><p>The first line contains an integer $t$ ($1 \leq t \leq 10^4$)&nbsp;— the number of input data sets in the test.</p><p>The description of each set of input data consists of three lines. The first line contains an integer $n$ ($1 \leq n \leq 2 \cdot 10^5$)&nbsp;— the length of the original array $a$. The second line contains $n$ integers $a_1$, $a_2$, ..., $a_n$ ($-10^9 \leq a_i \leq 10^9$)&nbsp;— the array elements themselves.</p><p>The third line has length $n$ and consists exclusively of the letters '<span class="tex-font-style-tt">B</span>' and/or '<span class="tex-font-style-tt">R</span>': $i$th character is '<span class="tex-font-style-tt">B</span>' if $a_i$ is colored blue, and is '<span class="tex-font-style-tt">R</span>' if colored red.</p><p>It is guaranteed that the sum of $n$ over all input sets does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>Print $t$ lines, each of which contains the answer to the corresponding test case of the input. Print <span class="tex-font-style-tt">YES</span> as an answer if the corresponding array can be transformed into a permutation, and <span class="tex-font-style-tt">NO</span> otherwise.</p><p>You can print the answer in any case (for example, the strings <span class="tex-font-style-tt">yEs</span>, <span class="tex-font-style-tt">yes</span>, <span class="tex-font-style-tt">Yes</span>, and <span class="tex-font-style-tt">YES</span> will be recognized as a positive answer).</p></div>

## Input

<p>The first line contains an integer $t$ ($1 \leq t \leq 10^4$)&nbsp;— the number of input data sets in the test.</p><p>The description of each set of input data consists of three lines. The first line contains an integer $n$ ($1 \leq n \leq 2 \cdot 10^5$)&nbsp;— the length of the original array $a$. The second line contains $n$ integers $a_1$, $a_2$, ..., $a_n$ ($-10^9 \leq a_i \leq 10^9$)&nbsp;— the array elements themselves.</p><p>The third line has length $n$ and consists exclusively of the letters '<span class="tex-font-style-tt">B</span>' and/or '<span class="tex-font-style-tt">R</span>': $i$th character is '<span class="tex-font-style-tt">B</span>' if $a_i$ is colored blue, and is '<span class="tex-font-style-tt">R</span>' if colored red.</p><p>It is guaranteed that the sum of $n$ over all input sets does not exceed $2 \cdot 10^5$.</p>

## Output

<p>Print $t$ lines, each of which contains the answer to the corresponding test case of the input. Print <span class="tex-font-style-tt">YES</span> as an answer if the corresponding array can be transformed into a permutation, and <span class="tex-font-style-tt">NO</span> otherwise.</p><p>You can print the answer in any case (for example, the strings <span class="tex-font-style-tt">yEs</span>, <span class="tex-font-style-tt">yes</span>, <span class="tex-font-style-tt">Yes</span>, and <span class="tex-font-style-tt">YES</span> will be recognized as a positive answer).</p>





```input1
8
4
1 2 5 2
BRBR
2
1 1
BB
5
3 1 4 2 5
RBRRB
5
3 1 3 1 3
RBRRB
5
5 1 5 1 5
RBRRB
4
2 2 2 2
BRBR
2
1 -2
BR
4
-2 -1 4 0
RRRR
```




```output1
YES
NO
YES
YES
NO
YES
YES
YES
```



## Note

<p>In the first test case of the example, the following sequence of moves can be performed:</p><ul> <li> choose $i=3$, element $a_3=5$ is blue, so we decrease it, we get $a=[1,2,4,2]$; </li><li> choose $i=2$, element $a_2=2$ is red, so we increase it, we get $a=[1,3,4,2]$; </li><li> choose $i=3$, element $a_3=4$ is blue, so we decrease it, we get $a=[1,3,3,2]$; </li><li> choose $i=2$, element $a_2=2$ is red, so we increase it, we get $a=[1,4,3,2]$. </li></ul><p>We got that $a$ is a permutation. Hence the answer is <span class="tex-font-style-tt">YES</span>.</p>
