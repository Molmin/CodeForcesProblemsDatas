## Description

<div><p>You're given an array $a$ of length $n$. You can perform the following operations on it:</p><ul> <li> choose an index $i$ $(1 \le i \le n)$, an integer $x$ $(0 \le x \le 10^6)$, and replace $a_j$ with $a_j+x$ for all $(1 \le j \le i)$, which means add $x$ to all the elements in the prefix ending at $i$. </li><li> choose an index $i$ $(1 \le i \le n)$, an integer $x$ $(1 \le x \le 10^6)$, and replace $a_j$ with $a_j \% x$ for all $(1 \le j \le i)$, which means replace every element in the prefix ending at $i$ with the remainder after dividing it by $x$. </li></ul><p>Can you make the array <span class="tex-font-style-bf">strictly increasing</span> in no more than $n+1$ operations?</p></div><div class="input-specification"><p>The first line contains an integer $n$ $(1 \le n \le 2000)$, the number of elements in the array $a$.</p><p>The second line contains $n$ space-separated integers $a_1$, $a_2$, $\dots$, $a_n$ $(0 \le a_i \le 10^5)$, the elements of the array $a$.</p></div><div class="output-specification"><p>On the first line, print the number of operations you wish to perform. On the next lines, you should print the operations.</p><p>To print an adding operation, use the format "$1$ $i$ $x$"; to print a modding operation, use the format "$2$ $i$ $x$". If $i$ or $x$ don't satisfy the limitations above, or you use more than $n+1$ operations, you'll get <span class="tex-font-style-it">wrong answer</span> verdict.</p></div>

## Input

<p>The first line contains an integer $n$ $(1 \le n \le 2000)$, the number of elements in the array $a$.</p><p>The second line contains $n$ space-separated integers $a_1$, $a_2$, $\dots$, $a_n$ $(0 \le a_i \le 10^5)$, the elements of the array $a$.</p>

## Output

<p>On the first line, print the number of operations you wish to perform. On the next lines, you should print the operations.</p><p>To print an adding operation, use the format "$1$ $i$ $x$"; to print a modding operation, use the format "$2$ $i$ $x$". If $i$ or $x$ don't satisfy the limitations above, or you use more than $n+1$ operations, you'll get <span class="tex-font-style-it">wrong answer</span> verdict.</p>





```input1
3
1 2 3

```




```input2
3
7 6 3

```




```output1
0
```




```output2
2
1 1 1
2 2 4

```



## Note

<p>In the first sample, the array is already increasing so we don't need any operations.</p><p>In the second sample:</p><p>In the first step: the array becomes $[8,6,3]$.</p><p>In the second step: the array becomes $[0,2,3]$.</p>
