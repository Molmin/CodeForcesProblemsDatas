## Description

<div><p><span class="tex-font-style-it">In fact, the problems E1 and E2 do not have much in common. You should probably think of them as two separate problems.</span></p><p>You are given an integer array $a[1 \ldots n] = [a_1, a_2, \ldots, a_n]$.</p><p>Let us consider an empty <a href="https://tinyurl.com/pfeucbux">deque</a> (double-ended queue). A deque is a data structure that supports adding elements to both the beginning and the end. So, if there are elements $[3, 4, 4]$ currently in the deque, adding an element $1$ to the beginning will produce the sequence $[\color{red}{1}, 3, 4, 4]$, and adding the same element to the end will produce $[3, 4, 4, \color{red}{1}]$.</p><p>The elements of the array are sequentially added to the initially empty deque, starting with $a_1$ and finishing with $a_n$. Before adding each element to the deque, you may choose whether to add it to the beginning or to the end.</p><p>For example, if we consider an array $a = [3, 7, 5, 5]$, one of the possible sequences of actions looks like this: </p><table class="tex-tabular"><tbody><tr><td class="tex-tabular-text-align-left">$\quad$ 1.</td><td class="tex-tabular-text-align-left">add $3$ to the beginning of the deque:</td><td class="tex-tabular-text-align-left">deque has a sequence $[\color{red}{3}]$ in it;</td></tr><tr><td class="tex-tabular-text-align-left">$\quad$ 2.</td><td class="tex-tabular-text-align-left">add $7$ to the end of the deque:</td><td class="tex-tabular-text-align-left">deque has a sequence $[3, \color{red}{7}]$ in it;</td></tr><tr><td class="tex-tabular-text-align-left">$\quad$ 3.</td><td class="tex-tabular-text-align-left">add $5$ to the end of the deque:</td><td class="tex-tabular-text-align-left">deque has a sequence $[3, 7, \color{red}{5}]$ in it;</td></tr><tr><td class="tex-tabular-text-align-left">$\quad$ 4.</td><td class="tex-tabular-text-align-left">add $5$ to the beginning of the deque:</td><td class="tex-tabular-text-align-left">deque has a sequence $[\color{red}{5}, 3, 7, 5]$ in it;</td></tr></tbody></table><p></p><p>Find the minimal possible number of inversions in the deque after the whole array is processed. </p><p>An <span class="tex-font-style-it">inversion</span> in sequence $d$ is a pair of indices $(i, j)$ such that $i &lt; j$ and $d_i &gt; d_j$. For example, the array $d = [5, 3, 7, 5]$ has exactly two inversions&nbsp;— $(1, 2)$ and $(3, 4)$, since $d_1 = 5 &gt; 3 = d_2$ and $d_3 = 7 &gt; 5 = d_4$.</p></div><div class="input-specification"><p>The first line contains an integer $t$ ($1 \leq t \leq 1000$)&nbsp;— the number of test cases.</p><p>The next $2t$ lines contain descriptions of the test cases. </p><p>The first line of each test case description contains an integer $n$ ($1 \le n \le 2 \cdot 10^5$)&nbsp;— array size. The second line of the description contains $n$ space-separated integers $a_i$ ($-10^9 \le a_i \le 10^9$)&nbsp;— elements of the array.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>Print $t$ lines, each line containing the answer to the corresponding test case. The answer to a test case should be a single integer&nbsp;— the minimal possible number of inversions in the deque after executing the described algorithm.</p></div>

## Input

<p>The first line contains an integer $t$ ($1 \leq t \leq 1000$)&nbsp;— the number of test cases.</p><p>The next $2t$ lines contain descriptions of the test cases. </p><p>The first line of each test case description contains an integer $n$ ($1 \le n \le 2 \cdot 10^5$)&nbsp;— array size. The second line of the description contains $n$ space-separated integers $a_i$ ($-10^9 \le a_i \le 10^9$)&nbsp;— elements of the array.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>Print $t$ lines, each line containing the answer to the corresponding test case. The answer to a test case should be a single integer&nbsp;— the minimal possible number of inversions in the deque after executing the described algorithm.</p>





```input1
6
4
3 7 5 5
3
3 2 1
3
3 1 2
4
-1 2 2 -1
4
4 5 1 3
5
1 3 1 3 2
```




```output1
2
0
1
0
1
2
```



## Note

<p>One of the ways to get the sequence $[5, 3, 7, 5]$ in the deque, containing only two inversions, from the initial array $[3, 7, 5, 5]$ (the first sample test case) is described in the problem statement. </p><p>Also, in this example, you could get the answer of two inversions by simply putting each element of the original array at the end of the deque. In this case, the original sequence $[3, 7, 5, 5]$, also containing exactly two inversions, will be in the deque as-is.</p>
