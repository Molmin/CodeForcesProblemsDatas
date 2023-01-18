## Description

<div><p>You are given an integer sequence $1, 2, \dots, n$. You have to divide it into two sets $A$ and $B$ in such a way that each element belongs to <span class="tex-font-style-bf">exactly one</span> set and $|sum(A) - sum(B)|$ is minimum possible.</p><p>The value $|x|$ is the absolute value of $x$ and $sum(S)$ is the sum of elements of the set $S$.</p></div><div class="input-specification"><p>The first line of the input contains one integer $n$ ($1 \le n \le 2 \cdot 10^9$).</p></div><div class="output-specification"><p>Print one integer — the minimum possible value of $|sum(A) - sum(B)|$ if you divide the initial sequence $1, 2, \dots, n$ into two sets $A$ and $B$.</p></div>

## Input

<p>The first line of the input contains one integer $n$ ($1 \le n \le 2 \cdot 10^9$).</p>

## Output

<p>Print one integer — the minimum possible value of $|sum(A) - sum(B)|$ if you divide the initial sequence $1, 2, \dots, n$ into two sets $A$ and $B$.</p>





```input1
3
```




```input2
5
```




```input3
6
```




```output1
0
```




```output2
1
```




```output3
1
```



## Note

<p>Some (not all) possible answers to examples:</p><p>In the first example you can divide the initial sequence into sets $A = \{1, 2\}$ and $B = \{3\}$ so the answer is $0$.</p><p>In the second example you can divide the initial sequence into sets $A = \{1, 3, 4\}$ and $B = \{2, 5\}$ so the answer is $1$.</p><p>In the third example you can divide the initial sequence into sets $A = \{1, 4, 5\}$ and $B = \{2, 3, 6\}$ so the answer is $1$.</p>
