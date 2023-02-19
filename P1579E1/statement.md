## Description

<div><p><span class="tex-font-style-it">In fact, the problems E1 and E2 do not have much in common. You should probably think of them as two separate problems.</span></p><p>A permutation $p$ of size $n$ is given. A <span class="tex-font-style-it">permutation</span> of size $n$ is an array of size $n$ in which each integer from $1$ to $n$ occurs exactly once. For example, $[1, 4, 3, 2]$ and $[4, 2, 1, 3]$ are correct permutations while $[1, 2, 4]$ and $[1, 2, 2]$ are not.</p><p>Let us consider an empty <a href="https://tinyurl.com/pfeucbux">deque</a> (double-ended queue). A deque is a data structure that supports adding elements to both the beginning and the end. So, if there are elements $[1, 5, 2]$ currently in the deque, adding an element $4$ to the beginning will produce the sequence $[\color{red}{4}, 1, 5, 2]$, and adding same element to the end will produce $[1, 5, 2, \color{red}{4}]$.</p><p>The elements of the permutation are sequentially added to the initially empty deque, starting with $p_1$ and finishing with $p_n$. Before adding each element to the deque, you may choose whether to add it to the beginning or the end.</p><p>For example, if we consider a permutation $p = [3, 1, 2, 4]$, one of the possible sequences of actions looks like this: </p><table class="tex-tabular"><tbody><tr><td class="tex-tabular-text-align-left">$\quad$ 1.</td><td class="tex-tabular-text-align-left">add $3$ to the end of the deque:</td><td class="tex-tabular-text-align-left">deque has a sequence $[\color{red}{3}]$ in it;</td></tr><tr><td class="tex-tabular-text-align-left">$\quad$ 2.</td><td class="tex-tabular-text-align-left">add $1$ to the beginning of the deque:</td><td class="tex-tabular-text-align-left">deque has a sequence $[\color{red}{1}, 3]$ in it;</td></tr><tr><td class="tex-tabular-text-align-left">$\quad$ 3.</td><td class="tex-tabular-text-align-left">add $2$ to the end of the deque:</td><td class="tex-tabular-text-align-left">deque has a sequence $[1, 3, \color{red}{2}]$ in it;</td></tr><tr><td class="tex-tabular-text-align-left">$\quad$ 4.</td><td class="tex-tabular-text-align-left">add $4$ to the end of the deque:</td><td class="tex-tabular-text-align-left">deque has a sequence $[1, 3, 2, \color{red}{4}]$ in it;</td></tr></tbody></table><p></p><p>Find the lexicographically smallest possible sequence of elements in the deque after the entire permutation has been processed. </p><p>A sequence $[x_1, x_2, \ldots, x_n]$ is <span class="tex-font-style-it">lexicographically smaller</span> than the sequence $[y_1, y_2, \ldots, y_n]$ if there exists such $i \leq n$ that $x_1 = y_1$, $x_2 = y_2$, $\ldots$, $x_{i - 1} = y_{i - 1}$ and $x_i &lt; y_i$. In other words, if the sequences $x$ and $y$ have some (possibly empty) matching prefix, and the next element of the sequence $x$ is strictly smaller than the corresponding element of the sequence $y$. For example, the sequence $[1, 3, 2, 4]$ is smaller than the sequence $[1, 3, 4, 2]$ because after the two matching elements $[1, 3]$ in the start the first sequence has an element $2$ which is smaller than the corresponding element $4$ in the second sequence.</p></div><div class="input-specification"><p>The first line contains an integer $t$ ($1 \leq t \leq 1000$)&nbsp;— the number of test cases.</p><p>The next $2t$ lines contain descriptions of the test cases. </p><p>The first line of each test case description contains an integer $n$ ($1 \le n \le 2 \cdot 10^5$)&nbsp;— permutation size. The second line of the description contains $n$ space-separated integers $p_i$ ($1 \le p_i \le n$; all $p_i$ are all unique)&nbsp;— elements of the permutation.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>Print $t$ lines, each line containing the answer to the corresponding test case. The answer to a test case should contain $n$ space-separated integer numbers&nbsp;— the elements of the lexicographically smallest permutation that is possible to find in the deque after executing the described algorithm.</p></div>

## Input

<p>The first line contains an integer $t$ ($1 \leq t \leq 1000$)&nbsp;— the number of test cases.</p><p>The next $2t$ lines contain descriptions of the test cases. </p><p>The first line of each test case description contains an integer $n$ ($1 \le n \le 2 \cdot 10^5$)&nbsp;— permutation size. The second line of the description contains $n$ space-separated integers $p_i$ ($1 \le p_i \le n$; all $p_i$ are all unique)&nbsp;— elements of the permutation.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>Print $t$ lines, each line containing the answer to the corresponding test case. The answer to a test case should contain $n$ space-separated integer numbers&nbsp;— the elements of the lexicographically smallest permutation that is possible to find in the deque after executing the described algorithm.</p>





```input1
5
4
3 1 2 4
3
3 2 1
3
3 1 2
2
1 2
2
2 1
```




```output1
1 3 2 4 
1 2 3 
1 3 2 
1 2 
1 2
```



## Note

<p>One of the ways to get a lexicographically smallest permutation $[1, 3, 2, 4]$ from the permutation $[3, 1, 2, 4]$ (the first sample test case) is described in the problem statement.</p>
