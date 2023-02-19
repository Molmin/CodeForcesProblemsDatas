## Description

<div><p><span class="tex-font-style-it">You like numbers, don't you? Nastia has a lot of numbers and she wants to share them with you! Isn't it amazing?</span></p><p>Let $a_i$ be how many numbers $i$ ($1 \le i \le k$) you have.</p><p>An $n \times n$ matrix is called beautiful if it contains <span class="tex-font-style-bf">all</span> the numbers you have, and for <span class="tex-font-style-bf">each</span> $2 \times 2$ submatrix of the original matrix is satisfied: </p><ol> <li> The number of occupied cells doesn't exceed $3$; </li><li> The numbers on each diagonal are distinct. </li></ol><p>Make a beautiful matrix of <span class="tex-font-style-bf">minimum</span> size.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10\,000$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains $2$ integers $m$ and $k$ ($1 \le m, k \le 10^5$)&nbsp;— how many numbers Nastia gave you and the length of the array $a$, respectively.</p><p>The second line of each test case contains $k$ integers $a_1, a_2, \ldots, a_{k}$ ($0 \le a_i \le m$, $a_1 + a_2 + \ldots + a_{k} = m$), where $a_i$ is how many numbers $i$ you have.</p><p>It's guaranteed that the sum of $m$ and $k$ in one test doesn't exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each $t$ test case print a single integer $n$&nbsp;— the size of the beautiful matrix.</p><p>In the next $n$ lines print $n$ integers $b_{i, j}$ ($0 \le b_{i, j} \le k$; if position is empty, print $b_{i, j} = 0$)&nbsp;— the beautiful matrix $b$ you made up. </p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10\,000$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains $2$ integers $m$ and $k$ ($1 \le m, k \le 10^5$)&nbsp;— how many numbers Nastia gave you and the length of the array $a$, respectively.</p><p>The second line of each test case contains $k$ integers $a_1, a_2, \ldots, a_{k}$ ($0 \le a_i \le m$, $a_1 + a_2 + \ldots + a_{k} = m$), where $a_i$ is how many numbers $i$ you have.</p><p>It's guaranteed that the sum of $m$ and $k$ in one test doesn't exceed $2 \cdot 10^5$.</p>

## Output

<p>For each $t$ test case print a single integer $n$&nbsp;— the size of the beautiful matrix.</p><p>In the next $n$ lines print $n$ integers $b_{i, j}$ ($0 \le b_{i, j} \le k$; if position is empty, print $b_{i, j} = 0$)&nbsp;— the beautiful matrix $b$ you made up. </p>





```input1
2
3 4
2 0 0 1
15 4
2 4 8 1
```




```output1
2
4 1
0 1
5
3 0 0 2 2
3 2 3 3 0
0 1 0 4 0
3 0 0 0 0
2 1 3 3 3
```



## Note

<p><span class="tex-font-style-bf">Note that $0$ in this problem represents a blank, not a number.</span></p><p>Examples of possible answers for the first test case:</p><p>$\begin{array}{cc} 1 &amp; 1 \\ 4 &amp; 0 \\ \end{array} \hspace{0,5cm} \begin{array}{cc} 1 &amp; 4 \\ 1 &amp; 0 \\ \end{array} \hspace{0,5cm} \begin{array}{cc} 4 &amp; 0 \\ 1 &amp; 1 \\ \end{array}$</p><p>Examples of <span class="tex-font-style-bf">not</span> beautiful matrices for the first test case:</p><p>$\begin{array}{cc} 1 &amp; 0 \\ 4 &amp; 1 \\ \end{array} \hspace{0,5cm} \begin{array}{cc} 4 &amp; 1 \\ 7 &amp; 1 \\ \end{array} \hspace{0,5cm} \begin{array}{cc} 1 &amp; 0 \\ 4 &amp; 0 \\ \end{array}$</p><p>The example of the <span class="tex-font-style-bf">not</span> beautiful matrix for the second test case:</p><p>$\begin{array}{cc} 3 &amp; 4 &amp; 0 &amp; 2 &amp; 2 \\ 3 &amp; 2 &amp; 3 &amp; 3 &amp; 0 \\ 0 &amp; 1 &amp; 0 &amp; 0 &amp; 0 \\ 3 &amp; 0 &amp; 0 &amp; 0 &amp; 0 \\ 2 &amp; 1 &amp; 3 &amp; 3 &amp; 3 \\ \end{array}$</p><p>Everything is okay, except the left-top submatrix contains $4$ numbers.</p>
