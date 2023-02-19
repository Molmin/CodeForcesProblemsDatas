## Description

<div><p>Sho has an array $a$ consisting of $n$ integers. An operation consists of choosing two distinct indices $i$ and $j$ and removing $a_i$ and $a_j$ from the array.</p><p>For example, for the array $[2, 3, 4, 2, 5]$, Sho can choose to remove indices $1$ and $3$. After this operation, the array becomes $[3, 2, 5]$. Note that after any operation, the length of the array is reduced by two.</p><p>After he made some operations, Sho has an array that has only <span class="tex-font-style-bf">distinct</span> elements. In addition, he made operations such that the resulting array is the <span class="tex-font-style-bf">longest</span> possible. </p><p>More formally, the array after Sho has made his operations respects these criteria: </p><ul> <li> No pairs such that ($i &lt; j$) and $a_i = a_j$ exist. </li><li> The length of $a$ is maximized. </li></ul><p>Output the length of the final array.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \leq t \leq 10^3$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($1 \leq n \leq 50$)&nbsp;— the length of the array.</p><p>The second line of each test case contains $n$ integers $a_i$ ($1 \leq a_i \leq 10^4$)&nbsp;— the elements of the array.</p></div><div class="output-specification"><p>For each test case, output a single integer&nbsp;— the length of the final array. Remember that in the final array, all elements are different, and its length is maximum.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \leq t \leq 10^3$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($1 \leq n \leq 50$)&nbsp;— the length of the array.</p><p>The second line of each test case contains $n$ integers $a_i$ ($1 \leq a_i \leq 10^4$)&nbsp;— the elements of the array.</p>

## Output

<p>For each test case, output a single integer&nbsp;— the length of the final array. Remember that in the final array, all elements are different, and its length is maximum.</p>





```input1
4
6
2 2 2 3 3 3
5
9 1 9 9 1
4
15 16 16 15
4
10 100 1000 10000
```




```output1
2
1
2
4
```



## Note

<p>For the first test case Sho can perform operations as follows: </p><ol> <li> Choose indices $1$ and $5$ to remove. The array becomes $[2, 2, 2, 3, 3, 3] \rightarrow [2, 2, 3, 3]$. </li><li> Choose indices $1$ and $4$ to remove. The array becomes $[2, 2, 3, 3] \rightarrow [2, 3]$. </li></ol> The final array has a length of $2$, so the answer is $2$. It can be proven that Sho cannot obtain an array with a longer length.<p>For the second test case Sho can perform operations as follows: </p><ol> <li> Choose indices $3$ and $4$ to remove. The array becomes $[9, 1, 9, 9, 1] \rightarrow [9, 1, 1]$. </li><li> Choose indices $1$ and $3$ to remove. The array becomes $[9, 1, 1] \rightarrow [1]$. </li></ol> The final array has a length of $1$, so the answer is $1$. It can be proven that Sho cannot obtain an array with a longer length.
