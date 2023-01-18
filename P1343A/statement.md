## Description

<div><p>Recently Vova found $n$ candy wrappers. He remembers that he bought $x$ candies during the first day, $2x$ candies during the second day, $4x$ candies during the third day, $\dots$, $2^{k-1} x$ candies during the $k$-th day. But there is an issue: Vova remembers neither $x$ nor $k$ but he is sure that $x$ and $k$ are positive integers and $k &gt; 1$.</p><p>Vova will be satisfied if you tell him <span class="tex-font-style-bf">any positive</span> integer $x$ so there is an integer $k&gt;1$ that $x + 2x + 4x + \dots + 2^{k-1} x = n$. It is guaranteed that at least one solution exists. <span class="tex-font-style-bf">Note that $k &gt; 1$</span>.</p><p>You have to answer $t$ independent test cases.</p></div><div class="input-specification"><p>The first line of the input contains one integer $t$ ($1 \le t \le 10^4$) — the number of test cases. Then $t$ test cases follow.</p><p>The only line of the test case contains one integer $n$ ($3 \le n \le 10^9$) — the number of candy wrappers Vova found. It is guaranteed that there is some positive integer $x$ and integer $k&gt;1$ that $x + 2x + 4x + \dots + 2^{k-1} x = n$.</p></div><div class="output-specification"><p>Print one integer — <span class="tex-font-style-bf">any positive</span> integer value of $x$ so there is an integer $k&gt;1$ that $x + 2x + 4x + \dots + 2^{k-1} x = n$.</p></div>

## Input

<p>The first line of the input contains one integer $t$ ($1 \le t \le 10^4$) — the number of test cases. Then $t$ test cases follow.</p><p>The only line of the test case contains one integer $n$ ($3 \le n \le 10^9$) — the number of candy wrappers Vova found. It is guaranteed that there is some positive integer $x$ and integer $k&gt;1$ that $x + 2x + 4x + \dots + 2^{k-1} x = n$.</p>

## Output

<p>Print one integer — <span class="tex-font-style-bf">any positive</span> integer value of $x$ so there is an integer $k&gt;1$ that $x + 2x + 4x + \dots + 2^{k-1} x = n$.</p>





```input1
7
3
6
7
21
28
999999999
999999984
```




```output1
1
2
1
7
4
333333333
333333328
```



## Note

<p>In the first test case of the example, one of the possible answers is $x=1, k=2$. Then $1 \cdot 1 + 2 \cdot 1$ equals $n=3$.</p><p>In the second test case of the example, one of the possible answers is $x=2, k=2$. Then $1 \cdot 2 + 2 \cdot 2$ equals $n=6$.</p><p>In the third test case of the example, one of the possible answers is $x=1, k=3$. Then $1 \cdot 1 + 2 \cdot 1 + 4 \cdot 1$ equals $n=7$.</p><p>In the fourth test case of the example, one of the possible answers is $x=7, k=2$. Then $1 \cdot 7 + 2 \cdot 7$ equals $n=21$.</p><p>In the fifth test case of the example, one of the possible answers is $x=4, k=3$. Then $1 \cdot 4 + 2 \cdot 4 + 4 \cdot 4$ equals $n=28$.</p>
