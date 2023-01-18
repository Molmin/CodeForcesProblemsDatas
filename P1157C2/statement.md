## Description

<div><p><span class="tex-font-style-bf">The only difference between problems C1 and C2 is that all values in input of problem C1 are distinct (this condition may be false for problem C2)</span>.</p><p>You are given a sequence $a$ consisting of $n$ integers.</p><p>You are making a sequence of moves. During each move you must take either the leftmost element of the sequence or the rightmost element of the sequence, write it down and remove it from the sequence. Your task is to write down a <span class="tex-font-style-bf">strictly</span> increasing sequence, and among all such sequences you should take the longest (the length of the sequence is the number of elements in it).</p><p>For example, for the sequence $[1, 2, 4, 3, 2]$ the answer is $4$ (you take $1$ and the sequence becomes $[2, 4, 3, 2]$, then you take the rightmost element $2$ and the sequence becomes $[2, 4, 3]$, then you take $3$ and the sequence becomes $[2, 4]$ and then you take $4$ and the sequence becomes $[2]$, the obtained increasing sequence is $[1, 2, 3, 4]$).</p></div><div class="input-specification"><p>The first line of the input contains one integer $n$ ($1 \le n \le 2 \cdot 10^5$) — the number of elements in $a$.</p><p>The second line of the input contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 2 \cdot 10^5$), where $a_i$ is the $i$-th element of $a$.</p></div><div class="output-specification"><p>In the first line of the output print $k$ — the maximum number of elements in a <span class="tex-font-style-bf">strictly</span> increasing sequence you can obtain.</p><p>In the second line print a string $s$ of length $k$, where the $j$-th character of this string $s_j$ should be '<span class="tex-font-style-tt">L</span>' if you take the leftmost element during the $j$-th move and '<span class="tex-font-style-tt">R</span>' otherwise. If there are multiple answers, you can print any.</p></div>

## Input

<p>The first line of the input contains one integer $n$ ($1 \le n \le 2 \cdot 10^5$) — the number of elements in $a$.</p><p>The second line of the input contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 2 \cdot 10^5$), where $a_i$ is the $i$-th element of $a$.</p>

## Output

<p>In the first line of the output print $k$ — the maximum number of elements in a <span class="tex-font-style-bf">strictly</span> increasing sequence you can obtain.</p><p>In the second line print a string $s$ of length $k$, where the $j$-th character of this string $s_j$ should be '<span class="tex-font-style-tt">L</span>' if you take the leftmost element during the $j$-th move and '<span class="tex-font-style-tt">R</span>' otherwise. If there are multiple answers, you can print any.</p>





```input1
5
1 2 4 3 2
```




```input2
7
1 3 5 6 5 4 2
```




```input3
3
2 2 2
```




```input4
4
1 2 4 3
```




```output1
4
LRRR
```




```output2
6
LRLRRR
```




```output3
1
R
```




```output4
4
LLRR
```



## Note

<p>The first example is described in the problem statement.</p>
