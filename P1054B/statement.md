## Description

<div><p>Initially Ildar has an empty array. He performs $n$ steps. On each step he takes a subset of integers already added to the array and appends the <span class="tex-font-style-tt">mex</span> of this subset to the array. </p><p>The <span class="tex-font-style-tt">mex</span> of an multiset of integers is the smallest <span class="tex-font-style-bf">non-negative</span> integer not presented in the multiset. For example, the <span class="tex-font-style-tt">mex</span> of the multiset $[0, 2, 3]$ is $1$, while the <span class="tex-font-style-tt">mex</span> of the multiset $[1, 2, 1]$ is $0$.</p><p>More formally, on the step $m$, when Ildar already has an array $a_1, a_2, \ldots, a_{m-1}$, he chooses some subset of indices $1 \leq i_1 &lt; i_2 &lt; \ldots &lt; i_k &lt; m$ (possibly, empty), where $0 \leq k &lt; m$, and appends the $mex(a_{i_1}, a_{i_2}, \ldots a_{i_k})$ to the end of the array.</p><p>After performing all the steps Ildar thinks that he might have made a mistake somewhere. He asks you to determine for a given array $a_1, a_2, \ldots, a_n$ the minimum step $t$ such that he has definitely made a mistake on at least one of the steps $1, 2, \ldots, t$, or determine that he could have obtained this array without mistakes.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($1 \leq n \leq 100\,000$)&nbsp;— the number of steps Ildar made.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \leq a_i \leq 10^9$)&nbsp;— the array Ildar obtained.</p></div><div class="output-specification"><p>If Ildar could have chosen the subsets on each step in such a way that the resulting array is $a_1, a_2, \ldots, a_n$, print $-1$.</p><p>Otherwise print a single integer $t$&nbsp;— the smallest index of a step such that a mistake was made on at least one step among steps $1, 2, \ldots, t$.</p></div>

## Input

<p>The first line contains a single integer $n$ ($1 \leq n \leq 100\,000$)&nbsp;— the number of steps Ildar made.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \leq a_i \leq 10^9$)&nbsp;— the array Ildar obtained.</p>

## Output

<p>If Ildar could have chosen the subsets on each step in such a way that the resulting array is $a_1, a_2, \ldots, a_n$, print $-1$.</p><p>Otherwise print a single integer $t$&nbsp;— the smallest index of a step such that a mistake was made on at least one step among steps $1, 2, \ldots, t$.</p>





```input1
4
0 1 2 1

```




```input2
3
1 0 1

```




```input3
4
0 1 2 239

```




```output1
-1
```




```output2
1
```




```output3
4
```



## Note

<p>In the first example it is possible that Ildar made no mistakes. Here is the process he could have followed.</p><ul> <li> $1$-st step. The initial array is empty. He can choose an empty subset and obtain $0$, because the <span class="tex-font-style-tt">mex</span> of an empty set is $0$. Appending this value to the end he gets the array $[0]$. </li><li> $2$-nd step. The current array is $[0]$. He can choose a subset $[0]$ and obtain an integer $1$, because $mex(0) = 1$. Appending this value to the end he gets the array $[0,1]$. </li><li> $3$-rd step. The current array is $[0,1]$. He can choose a subset $[0,1]$ and obtain an integer $2$, because $mex(0,1) = 2$. Appending this value to the end he gets the array $[0,1,2]$. </li><li> $4$-th step. The current array is $[0,1,2]$. He can choose a subset $[0]$ and obtain an integer $1$, because $mex(0) = 1$. Appending this value to the end he gets the array $[0,1,2,1]$. </li></ul><p>Thus, he can get the array without mistakes, so the answer is $-1$.</p><p>In the second example he has definitely made a mistake on the very first step, because he could not have obtained anything different from $0$.</p><p>In the third example he could have obtained $[0, 1, 2]$ without mistakes, but $239$ is definitely wrong.</p>
