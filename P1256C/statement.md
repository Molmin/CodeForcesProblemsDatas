## Description

<div><p>There is a river of width $n$. The left bank of the river is cell $0$ and the right bank is cell $n + 1$ (more formally, the river can be represented as a sequence of $n + 2$ cells numbered from $0$ to $n + 1$). There are also $m$ wooden platforms on a river, the $i$-th platform has length $c_i$ (so the $i$-th platform takes $c_i$ consecutive cells of the river). It is guaranteed that the sum of lengths of platforms does not exceed $n$.</p><p>You are standing at $0$ and want to reach $n+1$ somehow. If you are standing at the position $x$, you can jump to any position in the range $[x + 1; x + d]$. <span class="tex-font-style-bf">However</span> you don't really like the water so you can jump only to such cells that belong to some wooden platform. For example, if $d=1$, you can jump only to the next position (if it belongs to the wooden platform). <span class="tex-font-style-bf">You can assume that cells $0$ and $n+1$ belong to wooden platforms</span>.</p><p>You want to know if it is possible to reach $n+1$ from $0$ if you can move any platform to the left or to the right arbitrary number of times (possibly, zero) as long as they do not intersect each other (but two platforms can touch each other). It also means that you cannot change the relative order of platforms.</p><p><span class="tex-font-style-bf">Note that you should move platforms until you start jumping</span> (in other words, you first move the platforms and then start jumping).</p><p>For example, if $n=7$, $m=3$, $d=2$ and $c = [1, 2, 1]$, then one of the ways to reach $8$ from $0$ is follow:</p><center> <img class="tex-graphics" src="file://wYzmnXqL.png" style="max-width: 100.0%;max-height: 100.0%;">   <span class="tex-font-size-small">The first example: $n=7$.</span> </center></div><div class="input-specification"><p>The first line of the input contains three integers $n$, $m$ and $d$ ($1 \le n, m, d \le 1000, m \le n$) — the width of the river, the number of platforms and the maximum distance of your jump, correspondingly.</p><p>The second line of the input contains $m$ integers $c_1, c_2, \dots, c_m$ ($1 \le c_i \le n, \sum\limits_{i=1}^{m} c_i \le n$), where $c_i$ is the length of the $i$-th platform.</p></div><div class="output-specification"><p>If it is impossible to reach $n+1$ from $0$, print <span class="tex-font-style-tt">NO</span> in the first line. Otherwise, print <span class="tex-font-style-tt">YES</span> in the first line and the array $a$ of length $n$ in the second line — the sequence of river cells (excluding cell $0$ and cell $n + 1$).</p><p>If the cell $i$ does not belong to any platform, $a_i$ should be $0$. Otherwise, it should be equal to the index of the platform ($1$-indexed, platforms are numbered from $1$ to $m$ in order of input) to which the cell $i$ belongs.</p><p><span class="tex-font-style-bf">Note that</span> all $a_i$ equal to $1$ should form a contiguous subsegment of the array $a$ of length $c_1$, all $a_i$ equal to $2$ should form a contiguous subsegment of the array $a$ of length $c_2$, ..., all $a_i$ equal to $m$ should form a contiguous subsegment of the array $a$ of length $c_m$. The leftmost position of $2$ in $a$ should be greater than the rightmost position of $1$, the leftmost position of $3$ in $a$ should be greater than the rightmost position of $2$, ..., the leftmost position of $m$ in $a$ should be greater than the rightmost position of $m-1$.</p><p>See example outputs for better understanding.</p></div>

## Input

<p>The first line of the input contains three integers $n$, $m$ and $d$ ($1 \le n, m, d \le 1000, m \le n$) — the width of the river, the number of platforms and the maximum distance of your jump, correspondingly.</p><p>The second line of the input contains $m$ integers $c_1, c_2, \dots, c_m$ ($1 \le c_i \le n, \sum\limits_{i=1}^{m} c_i \le n$), where $c_i$ is the length of the $i$-th platform.</p>

## Output

<p>If it is impossible to reach $n+1$ from $0$, print <span class="tex-font-style-tt">NO</span> in the first line. Otherwise, print <span class="tex-font-style-tt">YES</span> in the first line and the array $a$ of length $n$ in the second line — the sequence of river cells (excluding cell $0$ and cell $n + 1$).</p><p>If the cell $i$ does not belong to any platform, $a_i$ should be $0$. Otherwise, it should be equal to the index of the platform ($1$-indexed, platforms are numbered from $1$ to $m$ in order of input) to which the cell $i$ belongs.</p><p><span class="tex-font-style-bf">Note that</span> all $a_i$ equal to $1$ should form a contiguous subsegment of the array $a$ of length $c_1$, all $a_i$ equal to $2$ should form a contiguous subsegment of the array $a$ of length $c_2$, ..., all $a_i$ equal to $m$ should form a contiguous subsegment of the array $a$ of length $c_m$. The leftmost position of $2$ in $a$ should be greater than the rightmost position of $1$, the leftmost position of $3$ in $a$ should be greater than the rightmost position of $2$, ..., the leftmost position of $m$ in $a$ should be greater than the rightmost position of $m-1$.</p><p>See example outputs for better understanding.</p>





```input1
7 3 2
1 2 1
```




```input2
10 1 11
1
```




```input3
10 1 5
2
```




```output1
YES
0 1 0 2 2 0 3
```




```output2
YES
0 0 0 0 0 0 0 0 0 1
```




```output3
YES
0 0 0 0 1 1 0 0 0 0
```



## Note

<p>Consider the first example: the answer is $[0, 1, 0, 2, 2, 0, 3]$. The sequence of jumps you perform is $0 \rightarrow 2 \rightarrow 4 \rightarrow 5 \rightarrow 7 \rightarrow 8$.</p><p>Consider the second example: it does not matter how to place the platform because you always can jump from $0$ to $11$.</p><p>Consider the third example: the answer is $[0, 0, 0, 0, 1, 1, 0, 0, 0, 0]$. The sequence of jumps you perform is $0 \rightarrow 5 \rightarrow 6 \rightarrow 11$.</p>
